<!-- Ineffable Voyage zine -->

<script lang="ts">
    import zine_image from '$lib/assets/voyage_zine/voyage_zine_couv.jpg';

    import agrumetendre_avatar from '$lib/assets/voyage_zine/avatars/agrumeTendre.jpg';
    import angellilou_avatar from '$lib/assets/voyage_zine/avatars/angellilou.jpg';
    import bucky_avatar from '$lib/assets/voyage_zine/avatars/bucky.png';
    import chouly_avatar from '$lib/assets/voyage_zine/avatars/chouly.png';
    import cybi_avatar from '$lib/assets/voyage_zine/avatars/cybi.png';
    import elnora_avatar from '$lib/assets/voyage_zine/avatars/elnora.jpg';
    import emi_avatar from '$lib/assets/voyage_zine/avatars/emi.jpg';
    import enelica_avatar from '$lib/assets/voyage_zine/avatars/enelica.png';
    import kaitas_avatar from '$lib/assets/voyage_zine/avatars/kaitas.jpg';
    import kay_avatar from '$lib/assets/voyage_zine/avatars/kay.png';
    import kimy_avatar from '$lib/assets/voyage_zine/avatars/kimy.png';
    import lambre_avatar from '$lib/assets/voyage_zine/avatars/lambre.png';
    import piki_avatar from '$lib/assets/voyage_zine/avatars/piki.jpg';
    import tsar_avatar from '$lib/assets/voyage_zine/avatars/tsar_2024_rond.png';
    import zevampirex_avatar from '$lib/assets/voyage_zine/avatars/zevampirex.jpg';

</script>

<!-- TODO : Add zine informations -->
<!-- <h1 class="text-xl text-center font-semibold">Ineffable Voyage zine</h1> -->

<!-- General div for the page -->
<div class="flex w-full flex-col items-center gap-15 mt-10 mb-10">


    <div class="card w-3/4 md:card-side bg-base-200 shadow-sm">
    <figure class="w-1/2">
        <img
        src={zine_image}
        alt="Ineffable Voyage zine cover" />
    </figure>
    <div class="card-body">
        <h2 class="card-title">Ineffable Voyage zine</h2>
        <p>A fanzine about Aziraphale and Crowley traveling </p>
        <div class="card-actions justify-end">
        <button class="btn btn-primary">Listen</button>
        </div>
    </div>
    </div>



    <!-- TODO : Add divider for participants -->
    <h1 class="divider divider-accent text-xl text-center font-semibold">Meet the team!</h1>

    <!-- TODO : Standardise avatar size ? -->
    <div class="grid sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-4 mr-10 ml-10 justify-items-center">

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={agrumetendre_avatar}
                alt="agrume tendre avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Agrume Tendre</h2>
                <p>Good Omens was on the watchlist of Agrume Tendre since 2019, but it's only with the release of season two that she watched the show. She fell in love very hard very fast with Crowley and Aziraphale, and proceeded to draw them constantly, starting with Inktober 2023 that she posted daily on TikTok. Good Omens and the fandom really motivated her to draw more and to write her own stories. Long live this beautiful fandom!</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={angellilou_avatar}
                alt="angellilou avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Angellilou</h2>
                <p>Angellilou has loved Good Omens since the 1st season but couldn't be active in the fandom due to studies. Once season 2 was released and they graduated, they could unleash the beast. And what a mistake to let that silly snake create what they want... In a year, Lilou (or Angel, who cares?), made an illustrated book about the Ineffable Romans and has a Vampire AU project on the way. Unstoppable, that's what they are.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={bucky_avatar}
                alt="bucky avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Bucky</h2>
                <p>French author and hopeless romantic, Bucky1984 has been adopted by the GO family (for love and eternityyyy) for nearly two years now, and had no choice but to write about our Ineffable Husbands since. Because, well... They are love incarnate! Keep faith in them and VAVOOM !</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={chouly_avatar}
                alt="chouly avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Chouly/Lychoubi</h2>
                <p>Obsessed with Good Omens and the husbands since 2019, the show is now literally part of her DNA. The ineffable lovely idiots help her improve in making comics, as she has already created over 7 on Good Omens, like her Atlantis AU. And this obsession does not seem to vanish any time soon... Ngk !</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={cybi_avatar}
                alt="cybi avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Cybi</h2>
                <p>A French artist who fell in love with Good Omens on a random Tuesday without knowing it (thank you, Pinterest) and who ended up being obsessed for 2 years now! But, I mean, who could resist Crowley and Aziraphale ?</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={elnora_avatar}
                alt="elnora avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Elnöra Whittaker</h2>
                <p>Elnöra is a Belgian artist who fell head over heels for the ineffable husbands and she hasn't gotten up since. She also sold her soul to her Reverse AU, Dusty Omens, that she's currently working on.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={emi_avatar}
                alt="emi avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Emeline Hofmann</h2>
                <p>Emi fell into the Good Omens spiral 25 years ago, when her best friend put the book in her hands. Of course, she saw the first season when it came out, excited by the fact that one of her favorite books was being adapted. But it's thanks to season 2 that she picked up her pencils again, after almost 10 years without touching them, and since then, she hasn't spent a day without drawing! Thank you, ineffable husbands!</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={enelica_avatar}
                alt="enelica avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Enelica</h2>
                <p>French artist who can't spend a second without thinking about the ineffable husbands. Currently trying not to be late for her latest fancomic "Meet me in Eden", even though she keeps adding "just one last detail!".</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={kaitas_avatar}
                alt="kaitas avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Kaitas</h2>
                <p>After years of obsessing over Doctor Who and an art block quite gigantic, Kaitas started a new obsession over Good Omens (no, it's not the same! 10 never landed into The House! Okay?).</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={kay_avatar}
                alt="kay avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Kay</h2>
                <p>After years of hearing about Good Omens, Kay finally decided to give it a go when Season 2 aired. Since then, the show has become a real source of inspiration for them, whether it's for drawing, cosplay, music, or crochet. It has also allowed them to meet an amazing community that is equally inspired and involved.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={kimy_avatar}
                alt="kimy avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Kimyekai</h2>
                <p>Started watchin Good Omens on a Sunday of November, ended up watching the two seasons in one go. They didn't sleep that night, but they never stopped drawing these two silies since then. They have taken over their life.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={lambre_avatar}
                alt="lambre avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Lambre</h2>
                <p>After rewatching the first season of Good Omens in 2023, Lambre fell down a rabbit hole of passion for the show that doesn't seem to have an end. Thanks to that, they found back their will to write and have too many fic ideas that they definitely can't write all at once.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={piki_avatar}
                alt="piki avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Piki</h2>
                <p>Traumatized (in the best way) by the end of season 2, Piki began her journey in the fandom heartbroken. She's forever grateful for the friends made along the way, and for Good Omens bringing back her passion for drawing, previously damaged by a burn out.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={tsar_avatar}
                alt="tsar avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Tsar</h2>
                <p>TsarPopcorn (also know as Tsarletta) was resting from a busy year (and a burnout) when they decided to watch a new series. Little did they know about how strong their love for Good Omens would be... When they are not obsessing over old man yaoi, they enjoy painting animals and starry nights.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

            <div class="card bg-base-200 w-5/6 shadow-sm">
            <figure>
                <img
                src={zevampirex_avatar}
                alt="zevampirex avatar" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Zevampirex</h2>
                <p>After watching Good Omens with a friend during lunch times at school, the life of ZeVampirex was changed forever. Unable to wait for season 2, she started imagining parallel universes of the show, full of silly animals. Maybe because Michael Sheen is really hard to draw, who knows... Will she be able to draw humans one day? Maybe. Will she stop being obsessed with the angel and the demon? Very unlikely.</p>
                <div class="card-actions justify-center">
                <button class="btn btn-primary">Social</button> 
                </div>
            </div>
            </div>

    </div>
</div>