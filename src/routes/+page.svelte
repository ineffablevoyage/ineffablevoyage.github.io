<!-- Home -->

<script lang="ts">
	import { resolve } from '$app/paths';

	import background from '$lib/assets/images_vrac/ballon_goodomensfanzine_field.jpg';
    import zine_image from '$lib/assets/images_vrac/temp_cuisine_title.png';

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
        </div>
    </div>
</div>