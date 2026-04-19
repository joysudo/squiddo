<script lang="ts">
    import "../app.css";
    let squiddo_name: string = "[Squiddo name]";
    let emotion: string = "emotion";
    let zone: string = "Twilight";
    let timer: `${number}:${number}` = "25:00";
</script>

<div class="tank-wrapper">
<div class="tank">
    <div class="tank-back"></div>
    <div class="sand"></div>
    <div class="tank-grid">
        <h1 class="mood">{squiddo_name} is feeling... <i>{emotion}</i>.</h1>
        <div class="pomodoro">
            <h4>Pomodoro</h4>
            <h3>{timer}</h3>
            <div class="buttons">
                <button>▷</button>
                <button>↻</button>
            </div>
        </div>
        <div class="tasks"><h4>Tasks</h4></div>
        <div class="zone"><h3>{zone}<br/><u><i>Zone</i></u></h3></div>
        <div class="badges"><h4>Badges</h4></div>
        <div class="edit friend-settings"><h4>Edit friends</h4></div>
        <div class="edit squiddo-settings"><h4>Edit squiddo</h4></div>
        <div class="squiddo">
            <div class="squiddo-wrapper">
                <div class="text-bubble">jfdksjfsd dfds dsfsd dfsd dsf sdffsd</div>
                 <svg xmlns="http://www.w3.org/2000/svg" width="255" height="287" viewBox="0 0 255 287" fill="none">
                    <path d="M124.554 1.71631C145.054 7.71767 223.221 88.0515 252.554 124.718C255.554 133.218 236.054 140.885 220.554 143.718C245.555 190.718 222.555 248.718 203.555 252.218C226.555 270.718 203.555 281.718 194.554 261.217C205.054 289.718 171.555 282.218 169.054 261.217C171.555 297.718 147.055 281.718 145.054 262.717C134.055 301.218 115.555 278.218 117.054 262.717C103.054 300.717 82.5547 283.22 94.0547 264.718C71.5547 298.718 65.555 272.218 79.0547 261.217C62.055 275.071 46.5547 261.217 67.5544 253.717C17.1544 244.917 28.5543 181.717 40.5543 151.217C40.5543 151.217 9.05469 151.217 1.55435 143.716C-1.20691 140.955 102.069 -4.86636 124.554 1.71631Z" fill="url(#paint0_linear_602_337)"/>
                    <path d="M124.554 1.71631C145.054 7.71767 223.221 88.0515 252.554 124.718C255.554 133.218 236.054 140.885 220.554 143.718C245.555 190.718 222.555 248.718 203.555 252.218C226.555 270.718 203.555 281.718 194.554 261.217C205.054 289.718 171.555 282.218 169.054 261.217C171.555 297.718 147.055 281.718 145.054 262.717C134.055 301.218 115.555 278.218 117.054 262.717C103.054 300.717 82.5547 283.22 94.0547 264.718C71.5547 298.718 65.555 272.218 79.0547 261.217C62.055 275.071 46.5547 261.217 67.5544 253.717C17.1544 244.917 28.5543 181.717 40.5543 151.217C40.5543 151.217 9.05469 151.217 1.55435 143.716C-1.20691 140.955 102.069 -4.86636 124.554 1.71631Z" fill="var(--cream)" fill-opacity="0.2"/>
                    <path d="M124.554 1.71631C145.054 7.71767 223.221 88.0515 252.554 124.718C255.554 133.218 236.054 140.885 220.554 143.718C245.555 190.718 222.555 248.718 203.555 252.218C226.555 270.718 203.555 281.718 194.554 261.217C205.054 289.718 171.555 282.218 169.054 261.217C171.555 297.718 147.055 281.718 145.054 262.717C134.055 301.218 115.555 278.218 117.054 262.717C103.054 300.717 82.5547 283.22 94.0547 264.718C71.5547 298.718 65.555 272.218 79.0547 261.217C62.055 275.071 46.5547 261.217 67.5544 253.717C17.1544 244.917 28.5543 181.717 40.5543 151.217C40.5543 151.217 9.05469 151.217 1.55435 143.716C-1.20691 140.955 102.069 -4.86636 124.554 1.71631Z" stroke="var(--navy)" stroke-width="2.5" vector-effect="non-scaling-stroke"/>
                    <path d="M198.055 160.718C198.055 155.718 193.655 145.718 180.055 145.718C164.055 145.718 163.055 156.218 163.055 159.718C163.055 163.218 163.555 173.218 180.555 173.218C194.155 173.218 198.055 164.718 198.055 160.718Z" fill="var(--mouth)" fill-opacity="0.25"/>
                    <path d="M122.555 160.491C122.555 155.4 117.903 145.218 103.526 145.218C86.6118 145.218 85.5547 155.909 85.5547 159.473C85.5547 163.036 86.0833 173.218 104.055 173.218C118.432 173.218 122.555 164.564 122.555 160.491Z" fill="var(--mouth)" fill-opacity="0.25"/>
                    <path d="M120.739 170.236C110.985 236.758 175.981 225.898 163.978 170.074C163.757 169.048 162.753 168.355 161.714 168.496C156.549 169.195 151.124 169.261 147.257 168.391C146.8 168.289 146.327 168.332 145.886 168.489C140.795 170.31 129.618 169.405 123.019 168.506C121.93 168.358 120.899 169.149 120.739 170.236Z" fill="var(--mouth)" stroke="var(--navy)" stroke-width="2.5" vector-effect="non-scaling-stroke"/>
                    <!-- eyes (could add vector-effect="non-scaling-stroke") -->
                    <path d="M156.822 145.95C155.846 144.974 154.263 144.974 153.287 145.95C152.311 146.927 152.311 148.51 153.287 149.486C154.263 150.462 155.846 150.462 156.822 149.486C157.799 148.51 157.799 146.927 156.822 145.95Z" fill="var(--navy)" stroke="var(--navy)" stroke-width="2" vector-effect="non-scaling-stroke"/>
                    <path d="M131.822 146.95C130.846 145.974 129.263 145.974 128.287 146.95C127.311 147.927 127.311 149.51 128.287 150.486C129.263 151.462 130.846 151.462 131.822 150.486C132.799 149.51 132.799 147.927 131.822 146.95Z" fill="var(--navy)" stroke="var(--navy)" stroke-width="2" vector-effect="non-scaling-stroke"/>
                    <path d="M179.555 154.718V162.218" stroke="var(--mouth)" stroke-width="4" stroke-linecap="round"/>
                    <path d="M107.555 154.218V161.718" stroke="var(--mouth)" stroke-width="4" stroke-linecap="round"/>
                    <path d="M186.055 155.218L187.555 162.218" stroke="var(--mouth)" stroke-width="4" stroke-linecap="round"/>
                    <path d="M100.555 154.218L98.0547 160.718" stroke="var(--mouth)" stroke-width="4" stroke-linecap="round"/>
                    <path d="M73.8358 86.2183C77.3087 86.2183 78.7615 83.959 79.4076 81.3096C80.235 77.9165 77.4563 74.1577 73.9811 74.219C70.8313 74.2746 68.5547 77.4916 68.5547 80.2187C68.5547 82.9459 69.4946 86.2183 73.8358 86.2183Z" fill="var(--cream)"/>
                    <path d="M65.4353 94.2183C67.3296 94.2183 68.1221 93.0886 68.4744 91.7639C68.9258 90.0674 67.4101 88.188 65.5146 88.2186C63.7965 88.2464 62.5547 89.8549 62.5547 91.2185C62.5547 92.5821 63.0674 94.2183 65.4353 94.2183Z" fill="var(--cream)"/>
                    <defs>
                        <linearGradient id="paint0_linear_602_337" x1="121.189" y1="-50.7086" x2="121.189" y2="389.718" gradientUnits="userSpaceOnUse">
                            <stop stop-color="var(--lavender)"/>
                            <stop offset="1" stop-color="var(--sky)"/>
                        </linearGradient>
                    </defs>
                </svg>
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
        --mouth: #DF8D99;
    }

    button {
        flex: 1;
        border-radius: 10px;
        padding: 2%;
        border: transparent;
        color: var(--navy);
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
        /* height: calc(90vh - min(10vw, 10vh)); */
        inset: min(10vw, 10vh) min(5vw, 5vh);
        z-index: 2;
        display: grid;
        gap: 1rem;
        grid-template-columns: 2fr 2fr 2fr 1.5fr;
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
        .squiddo-wrapper {
            height: 100%;
            position: relative;
            display: flex;
            flex-direction: row-reverse !important;
            align-items: flex-start !important;
            gap: 1vw !important;
            animation: float 4s ease-in-out alternate infinite !important;
        }
        .squiddo svg {
            max-height: 18vh;
        }
        .text-bubble {
            max-height: 100% !important;
            aspect-ratio: none;
            width: 100% !important;
        }
    }

    .tank-grid > *:not(:first-child) {
        /* opacity: 0.2; */
        border: 3px solid var(--navy);
        border-radius: 15px;
        padding: min(2vw, 2vh);
    }

    .tank-grid > * > h4 {
        font-size: clamp(1.094rem, 0.865rem + 1.15vi, 1.67rem);
        text-decoration: underline; 
        font-family: 'Instrument Sans', sans-serif;
    }

    .mood { 
        grid-area: A; 
        font-size: clamp(2rem, min(8vw, 8vh), 4rem);
        line-height: 0.67;
    }

    .pomodoro { 
        grid-area: B; 
        background-color: color-mix(in srgb, var(--sand), transparent 30%);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .pomodoro h3 {
        /* font-size: clamp(1.709rem, 1.181rem + 2.64vi, 2.969rem); */
        /* font-size: clamp(2.671rem, 1.541rem + 5.65vi, 5.278rem); */
        font-size: clamp(2.136rem, 1.37rem + 3.83vi, 3.959rem);
        margin: 0 auto;
        font-style: italic;
    }

    .pomodoro .buttons {
        display: flex;
        width: 100%;
        gap: 0.5rem;
    }

    .pomodoro .buttons button {
        background-color: color-mix(in srgb, var(--navy), transparent 93%);
    }

    .pomodoro .buttons button:first-child {
        background-color: color-mix(in srgb, var(--cream), transparent 50%);
        transition: filter 0.2s ease;
    }

    .pomodoro .buttons button:first-child:hover {
        filter: brightness(0.9);
    }

    .pomodoro .buttons button:first-child:active {
        filter: brightness(0.8);
    }

    .pomodoro .buttons button:last-child:hover {
        transition: background-color 0.2s ease;
    }

    .pomodoro .buttons button:last-child:hover {
        background-color: color-mix(in srgb, var(--navy), transparent 85%);
    }

    .pomodoro .buttons button:last-child:active {
        background-color: color-mix(in srgb, var(--navy), transparent 80%);
    }


    .tasks { 
        grid-area: C; 
        background-color: color-mix(in srgb, var(--lavender), transparent 30%);
    }

    .zone { 
        grid-area: D; 
        background-color: color-mix(in srgb, 
            color-mix(in srgb, var(--navy), var(--cream) 65%), 
        transparent 20%);
    }

    .zone h3 {
        font-size: clamp(1.368rem, 1.015rem + 1.76vi, 2.227rem);
        /* font-size: clamp(1.709rem, 1.181rem + 2.64vi, 2.969rem); */
        line-height: 0.75;
    }

    .badges { 
        grid-area: E; 
        background-color: color-mix(in srgb, 
            color-mix(in srgb, var(--navy), var(--sky) 75%), 
        transparent 50%);
        font-size: clamp(0.875rem, 0.741rem + 0.67vi, 1.25rem);
    }

    .edit {
        background-color: color-mix(in srgb, 
            color-mix(in srgb, var(--navy), var(--cream)), 
        transparent 30%);
        font-size: clamp(0.875rem, 0.741rem + 0.67vi, 1.25rem);
    }
    
    .friend-settings { 
        grid-area: F; 
    }

    .squiddo-settings { 
        grid-area: G; 
    }

    .squiddo { 
        grid-area: H; 
        border: none !important;
        position: relative;
        display: flex;
        justify-content: center;
    }

    .squiddo-wrapper {
        max-width: 100%;
        position: absolute;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: max(1rem, 3vw);
        animation: float 10s ease-in-out alternate infinite;
        max-height: 100%;
        /* height: fit-content; */
    }

    @keyframes float {
        0% {
            top: 0;
            transform: translateY(0);
        }
        100% {
            top: 100%;
            transform: translateY(-100%);
        }
    }

    .squiddo svg {
        position: relative;
        display: block;
        max-width: 100%;
        flex: 1 1 auto;
        min-height: 2rem;
    }

    .text-bubble {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;
        font-size: clamp(0.75rem, 1.5vw, 1rem);
        line-height: 1;
        width: auto;
        padding: 5%;
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
        right: 50%;
        top: 100%;
        width: 10%;
        height: 20%;
        background-color: var(--cream);
        border-radius: 0 0 50% 50% / 0 0 100% 100%;
        border-left: 3px solid var(--navy);
        border-right: 3px solid var(--navy);
        border-bottom: 3px solid var(--navy);
        /* transform: rotate(4deg) translateY(-0.5px); */
    }
</style>