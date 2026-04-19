<script lang="ts">
    import "../app.css";
</script>

<div class="tank-wrapper">
<div class="tank">
    <div class="tank-back"></div>
    <div class="sand"></div>
    <div class="tank-grid">
        <h1 class="mood">Squid name is feeling... <i>emotion</i>.</h1>
        <div class="pomodoro">Pomodoro</div>
        <div class="tasks">Tasks</div>
        <div class="zone">Zone</div>
        <div class="badges">Badges</div>
        <div class="edit friend-settings">Edit friends</div>
        <div class="edit squiddo-settings">Edit squiddo</div>
        <div class="squiddo">
            <div class="text-bubble">
                <p>jfdksjfsd dfds dsfsd dfsd dsf sdffsd</p>
            </div>
        </div>
    </div>
</div>
</div>

<style lang="css">
    :root {
        /* tank borders */
        --thick: min(3vw, 3vh);
        --len: min(7vw, 7vh);
    }

    .tank {
        position: relative;
        width: 90vw;
        height: calc(90vh + var(--thick) / 2);
        background-color: var(--sky);
        /* margin: auto; */
        border-radius: 15px;
        border: 3px solid var(--navy);
        overflow: hidden;
        z-index: 0;
        border-top: calc(var(--thick) + 3px) solid var(--navy);
    }

    .tank::before {
        /* highlight on tank */
        content: "";
        display: block;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 70%;
        background-color: var(--cream);
        border-radius: 0 0 50% 50% / 0 0 30% 30%;
        opacity: 0.3;
        z-index: -1;
    }

    .tank-back {
        z-index: 1;
        width: 72%;
        height: 100%;
        margin: auto;
        border-left: 3px solid var(--navy);
        border-right: 3px solid var(--navy);
    }

    .sand {
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 20%;
        background-color: antiquewhite;
        border-radius: 15px 15px 0 0;
        transform: perspective(10rem) rotateX(20deg);
        transform-origin: bottom;
        border-left: 4px solid var(--navy);
        border-right: 4px solid var(--navy);
        border-top: 4px solid var(--navy);
    }

    .tank-wrapper {
        /* this is just for the borders bc actual tank has overflow hidden */
        position: relative;
        display: flex;
        justify-content: center;
        /* align-items: center; */
        z-index: 50;
        width: calc(90vw + var(--thick));
        height: calc(90vh + var(--thick));
        margin: auto;
    }

    .tank-wrapper::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: var(--len); 
        height: var(--thick);
        background: var(--navy);
        border-radius: 999px;


        box-shadow: 
            calc(calc(90vw + var(--thick)) - var(--len)) 0 0 0 var(--navy),
            0 calc(calc(90vh + var(--thick)) - var(--thick)) 0 0 var(--navy),
            calc(calc(90vw + var(--thick)) - var(--len)) calc(calc(90vh + var(--thick)) - var(--thick)) 0 0 var(--navy);
        z-index: 20;
    }

    .tank-wrapper::after {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: var(--thick);
        height: var(--len);
        background: var(--navy);
        border-radius: 999px;
        box-shadow: 
            calc(calc(90vw + var(--thick)) - var(--thick)) 0 0 0 var(--navy), /* top right */
            0 calc(calc(90vh + var(--thick)) - var(--len)) 0 0 var(--navy), /* bottom left */
            calc(calc(90vw + var(--thick)) - var(--thick)) calc(calc(90vh + var(--thick)) - var(--len)) 0 0 var(--navy); /* bottom right */
    }

    .tank-grid {
        position: absolute;
        inset: min(5vw, 5vh);
        z-index: 2;
        display: grid;
        gap: 1rem;
        grid-template-columns: 2.5fr 2fr 2fr 1.5fr;
        grid-template-rows: auto repeat(2, 1fr) auto;
        grid-template-areas:
            "H A A A"
            "H B C D"
            "H E E D"
            "H F G D";
    }

    @media (max-width: 834px) {
        .tank-grid {
            grid-template-columns: 1fr 1fr;
            grid-template-rows: auto repeat(3, 1fr) auto;
            grid-template-areas:
                "A A"
                "B D"
                "C D"
                "H E"
                "F G";
        }
        /* add squid logic changing here too */
    }

    .tank-grid > *:not(:first-child) {
        /* opacity: 0.2; */
        border: 3px solid var(--navy);
        border-radius: 15px;
        padding: min(2vw, 2vh);
    }

    .mood { 
        grid-area: A; 
    }

    .pomodoro { 
        grid-area: B; 
        background-color: color-mix(in srgb, var(--sand), transparent 30%);
    }

    .tasks { 
        grid-area: C; 
        background-color: color-mix(in srgb, var(--lavender), transparent 30%);
    }

    .zone { 
        grid-area: D; 
        background-color: color-mix(in srgb, 
            color-mix(in srgb, var(--navy), var(--cream) 60%), 
        transparent 30%);
    }

    .badges { 
        grid-area: E; 
        background-color: color-mix(in srgb, var(--sky), transparent 30%);
    }

    .edit {
        background-color: color-mix(in srgb, 
            color-mix(in srgb, var(--navy), var(--cream)), 
        transparent 30%);
    }
    
    .friend-settings { 
        grid-area: F; 
    }

    .squiddo-settings { 
        grid-area: G; 
    }

    .squiddo { 
        grid-area: H; 
    }

    .text-bubble {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;
        font-size: clamp(0.75rem, 1.5vw, 1rem);
        line-height: 1;
        width: 50%;
        aspect-ratio: 1.5;
        max-height: 50%;
        border-radius: 30% / 45%;
        background-color: var(--cream);
        border: 3px solid var(--navy);
        overflow: visible;
    }

    .text-bubble::after {
        content: "";
        position: absolute;
        left: 50%;
        top: 100%;
        width: 10%;
        height: 20%;
        background-color: var(--cream);
        border-radius: 0 0 50% 50% / 0 0 100% 100%;
        border-left: 3px solid var(--navy);
        border-right: 3px solid var(--navy);
        border-bottom: 3px solid var(--navy);
        transform: rotate(4deg) translateY(-0.5px);
    }
</style>