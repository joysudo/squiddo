<script lang="ts">
    import "../app.css";
</script>

<div class="frame">
<div class="tank">
    <div class="tank-back"></div>
    <div class="sand"></div>
</div>
</div>

<style lang="css">
    :root {
        --thick: min(3vw, 3vh);
        --len: min(10vw, 10vh);
        --navy: #0A3474;
        --cream: #F8F5E9;
        --sand: #F9EABF;
        --sky: #C2E8F3;
        --lavender: #928DDF;
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

.frame {
    position: relative;
    display: flex;
    justify-content: center;
    /* align-items: center; */
    z-index: 50;
    width: calc(90vw + var(--thick));
    height: calc(90vh + var(--thick));
    margin: auto;
}

.frame::before {
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

.frame::after {
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
</style>