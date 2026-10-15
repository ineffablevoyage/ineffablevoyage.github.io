<!-- Home -->

<script lang="ts">
    import { onMount, onDestroy, afterUpdate } from 'svelte';
    import { resolve } from "$app/paths";

	import background from "$lib/assets/images_vrac/ballon_goodomensfanzine_field.jpg";
    import zine_image from "$lib/assets/cuisine_zine/cuisine_cover.png";

    // Countdown variables and function
    let current_date = new Date().getTime(); // Current date UTC in milliseconds
    let end_date = new Date("2026-11-15T00:00:00").getTime(); // End date UTC in milliseconds
    let time_left = end_date - current_date;
    let days = Math.floor(time_left / (1000 * 60 * 60 * 24));
    let hours = Math.floor((time_left /  (1000 * 60 * 60))) % 24;
    let minutes = Math.floor((time_left / (1000 * 60))) % 60;
    let seconds = Math.floor((time_left / 1000)) % 60;

    function remaningTime() {
        current_date = new Date().getTime();
        time_left = end_date - current_date;
        days = Math.floor(time_left / (1000 * 60 * 60 * 24));
        hours = Math.floor((time_left /  (1000 * 60 * 60))) % 24;
        minutes = Math.floor((time_left / (1000 * 60))) % 60;
        seconds = Math.floor((time_left / 1000)) % 60;

        document.getElementById('days')!.style.setProperty('--value', days.toString());
        document.getElementById('hours')!.style.setProperty('--value', hours.toString());
        document.getElementById('min')!.style.setProperty('--value', minutes.toString());
        document.getElementById('sec')!.style.setProperty('--value', seconds.toString());
    }

    onMount(() => {
        setInterval(() => {
                if(days > 0 || hours > 0 || minutes > 0 || seconds > 0) {
                    remaningTime();
                }
        }, 1000)
    })
</script>

<!-- TODO : Change presentation depending on screen size by using the hidden attribute in the same way as for the navbar -->


<div
  class="flex-1 hero min-h-full"
  style="background-image: url({background});"
    >
    <!-- <div class="hero-overlay"></div> -->
    <div class="hero-content text-neutral-content text-center">

            <div class="card md:card-l lg:card-side bg-base-100 shadow-sm max:w-5/6">
                <div class="card-body">
                    <h2 class="card-title">Ineffable Cuisine zine</h2>
                    <p>Comming soon.</p>
                    
                    <div class="grid auto-cols-max grid-flow-col gap-5 text-center">
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span id="days" style="--value:{days};" aria-live="polite" >{days}</span>
                            </span>
                            days
                        </div>
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span id="hours" style="--value:{hours};" aria-live="polite">{hours}</span>
                            </span>
                            hours
                        </div>
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span id="min" style="--value:{minutes};" aria-live="polite">{minutes}</span>
                            </span>
                            min
                        </div>
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span id="sec" style="--value:{seconds};" aria-live="polite">{seconds}</span>
                            </span>
                            sec
                        </div>
                    </div>

                    <!-- TODO : Add a "preorder button next to "learn more" for people that want to get the zine now -->
                    <div class="card-actions justify-center">
                        <a class="btn btn-primary" href="{resolve("/ineffableCuisineZine")}">Learn more</a>
                    </div>
                </div>
                <div class="hover-3d">
                    <!-- content -->
                    <figure class="md:w-100">
                        <enhanced:img src={zine_image} alt="fanzine cover" />
                    </figure>
                    <!-- 8 empty divs needed for the 3D effect -->
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                </div>
            </div>
    </div>
</div>
