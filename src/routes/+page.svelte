<!-- <div class="main_container">
    <div class="title">
        <h1>[Main page]</h1>
    </div>
    <div class="main_content">


    </div>
</div> -->

<script lang="ts">
	import { resolve } from '$app/paths';

	import background from '$lib/assets/images/ballon_goodomensfanzine_field.jpg';
    import zine_image from '$lib/assets/images/temp_cuisine_title.png';

</script>

<div
  class="hero min-h-screen"
  style="background-image: url('{background}');"
>
    <!-- <div class="hero-overlay"></div> -->
    <div class="hero-content text-neutral-content text-center">
        <div class="max-w-xl">
            <div class="card card-side bg-base-100 shadow-sm">
                <div class="card-body">
                    <h2 class="card-title">Ineffable Cuisine zine</h2>
                    <p>Comming soon.</p>
                    <div class="card-actions justify-end">
                    <a class="btn btn-primary" href="{resolve("/ineffableCuisineZine")}">Learn more</a>
                    </div>
                </div>
                <!-- <figure>
                    <img
                    src="{zine_image}"
                    alt="fanzine cover" />
                </figure> -->
                <div class="hover-3d">
                    <!-- content -->
                    <figure class="w-100">
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
            <!-- <h1 class="mb-5 text-5xl font-bold">Ineffable Cuisine</h1>
            <p class="mb-5">
                A new fanzine made by the people that made Ineffable voyage. 
            </p>
            <button class="btn btn-primary">Preorder soon !</button> -->
        </div>
    </div>
</div>

<!-- <div class="hero bg-base-200 min-h-screen">
    <div class="hero-content flex-col lg:flex-row-reverse">
        <img
        src="{zine_image}"
        class="max-w-sm rounded-lg shadow-2xl"
        alt=""
        />
        <div>
            <h1 class="text-5xl font-bold">Ineffable Cuisine Fanzine </h1>
            <p class="py-6">
                A new fanzine following the Ineffable Voyage one made by the same group ! New arts, new fics, and even more sweet !
            </p>
            <button class="btn btn-primary">Preorder soon !</button>
        </div>
    </div>
</div> -->