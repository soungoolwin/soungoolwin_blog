<template>
    <div class="timeline">
        <div class="tl-content tl-content-active">
            <div class="tl-header">
                <span class="tl-marker"></span>
                <p class="tl-title">Barlote</p>

                <p>
                    <time class="tl-time" datetime="2023-09-14">
                        Sept 14, 2023
                    </time>
                </p>
            </div>

            <div class="tl-body">
                <p>
                    I am currently working as intern laravel developer at
                    <em><b>Barlote</b></em
                    >.
                </p>
            </div>
        </div>
        <div class="tl-content tl-content-active">
            <div class="tl-header">
                <span class="tl-marker"></span>
                <p class="tl-title">Technophilia Lab</p>

                <p>
                    <time class="tl-time" datetime="2023-01-01">
                        January 1, 2023
                    </time>
                </p>
            </div>

            <div class="tl-body">
                <p>I also run as a freelance web developer(Side Job).</p>
            </div>
        </div>
        <!-- <div class="tl-content">
                <div class="tl-header">
                    <span class="tl-marker"></span>
                    <p class="tl-title"></p>

                    <p>
                        <time class="tl-time" datetime="2023-06-14">
                            Oct, 2022
                        </time>
                    </p>
                </div>

                <div class="tl-body">
                    <p>I got</p>
                </div>
            </div> -->
    </div>
</template>

<script>
export default {};
</script>

<style>
*,
*::after,
*::before {
    box-sizing: border-box;

    margin: 0;
    padding: 0;
}

p {
    line-height: 1.8;
}

time {
    line-height: 1.6;
}

body {
    min-width: 375px;

    font-family: "Poppins", sans-serif;

    background-color: #f1f1f1;
    color: #1a1a1a;
}

main {
    min-height: 100vh;

    display: grid;
    place-content: center;

    padding: 1rem;
}

/* ===================== */
/* ===================== */

/* Timeline */
/* Code Here ↓ */

.timeline {
    padding: 3rem 2rem;

    max-width: 460px;
    border-radius: 12px;

    background-color: white;
    box-shadow: 0 4px 25px -20px rgba(0, 0, 0.2);
}

.tl-content .tl-header,
.tl-content .tl-body {
    padding-left: 25.6px;

    border-left: 3px solid gainsboro;
}

.tl-body {
    padding-bottom: 1rem;
}

.tl-content:last-child .tl-body {
    border-left: 3px solid transparent;
}

.tl-header {
    position: relative;
    display: grid;

    padding-top: 1rem;
    padding-bottom: 1rem;
}

.tl-title {
    font-weight: 600;
    font-size: 1em;

    border-bottom: 1px solid gainsboro;
}

.tl-time {
    font-size: 0.7em;
}

.tl-marker {
    display: block;
    position: absolute;

    width: 16px;
    height: 16px;
    border-radius: 50% / 50%;

    background: gainsboro;

    left: -1.1rem;
    top: 50%;

    transform: translate(50%, -50%);
}

.tl-content-active .tl-marker {
    padding: 1.6px;

    left: -1.25rem;

    width: 18px;
    height: 18px;

    border: 2px solid limegreen;

    background-color: limegreen;
    background-clip: content-box;

    box-shadow: 0 0 15px -2px limegreen;
}

.tl-content-active .tl-title {
    font-weight: 700;

    color: green;
}
</style>
