<!-- Ineffable Cuisine zine -->

<script lang="ts">
    import zine_image from '$lib/assets/cuisine_zine/cusine_cover_sketch.png';

</script>

<!-- TODO : Add zine informations -->
<!-- <h1 class="text-xl text-center font-semibold">Ineffable Voyage zine</h1> -->

<!-- General div for the page -->
<div class="flex w-full flex-col items-center gap-15 mt-10 mb-10">

    <div class="card w-5/6 lg:w-2/3 md:card-side bg-base-200 shadow-sm">
    <figure>
        <img
        src={zine_image}
        alt="Ineffable Voyage zine cover" />
    </figure>
    <div class="card-body md:min-w-1/2"> <!-- TODO : Once the text is added, test best width for this element-->
        <h2 class="card-title">Ineffable Cuisine zine</h2>
        <p>A fanzine about Aziraphale and Crowley discovering various food across time and space</p>
        <div class="card-actions justify-end">
        <!-- <button class="btn btn-primary">Listen</button> -->
        </div>
    </div>
    </div>



    <!-- TODO : Add divider for participants -->
    <h1 class="divider divider-accent text-xl text-center font-semibold">Meet the team!</h1>

    <!-- TODO : Standardise avatar size ? -->
    <!-- TODO : Add everyone social ! (yeay T^T) -->
    <div class="grid sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-4 mr-10 ml-10 justify-items-center">

    </div>
</div>