<!-- Home -->

<script lang="ts">
    import { resolve } from '$app/paths';

	import background from '$lib/assets/images_vrac/ballon_goodomensfanzine_field.jpg';
    import zine_image from '$lib/assets/cuisine_zine/cusine_cover_sketch.png';
</script>

<!-- TODO : Change presentation depending on screen size by using the hidden attribute in the same way as for the navbar -->


<div
  class="flex-1 hero min-h-full"
  style="background-image: url('{background}');"
>
    <!-- <div class="hero-overlay"></div> -->
    <div class="hero-content text-neutral-content text-center">

            <div class="card md:card-l lg:card-side bg-base-100 shadow-sm max:w-5/6">
                <div class="card-body">
                    <h2 class="card-title">Ineffable Cuisine zine</h2>
                    <p>Comming soon.</p>
                    
                    <!-- <div class="grid auto-cols-max grid-flow-col gap-5 text-center justify-center">
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span style="--value:15;" aria-live="polite" aria-label="15">15</span>
                            </span>
                            days
                        </div>
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span style="--value:10;" aria-live="polite" aria-label="10">10</span>
                            </span>
                            hours
                        </div>
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span style="--value:24;" aria-live="polite" aria-label="24">24</span>
                            </span>
                            min
                        </div>
                        <div class="flex flex-col">
                            <span class="countdown font-mono text-5xl">
                            <span style="--value:59;" aria-live="polite" aria-label="59">59</span>
                            </span>
                            sec
                        </div>
                    </div> -->
            
                    <div class="card-actions justify-center">
                        <a class="btn btn-primary" href="{resolve("/ineffableCuisineZine")}">Learn more</a>
                    </div>
                </div>
                <div class="hover-3d">
                    <!-- content -->
                    <figure class="md:w-100">
                        <img src="{zine_image}" alt="fanzine cover" />
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