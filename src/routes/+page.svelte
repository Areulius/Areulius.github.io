<script>
    import Navbar from './navbar.svelte'

    let value = $state(16);
</script>

<div class="bg square" style="--amount-of-beams: {value};">
    <Navbar />

    <div>
        <h1>Welcome to Valdis (again)</h1>
    </div>

    <div class="sun"></div>

    <div class="range-slider">
        <input class="input-range" aria-orientation="vertical" type="range" bind:value={value} min="2" max="1000">
        <span class="range-value"></span>
    </div> 
</div>


<style>
    h1 {
        color :black;
    }

    .bg {
        width: 100vw;
        height: 100vh;
    }

    .range-slider {
        background-color: #DD0303;
        float:right;
        transform: rotate(-90deg);
    }

    .square {
        justify-content: center;
        align-items: center;
        background-color: blue;

        --yellow-beam: #FAB12F;
        --beige-beam: #FEF3E2;
        --red-beam: #DD0303;

        image-resolution: 300dpi;
        background-image: repeating-conic-gradient(
            var(--beige-beam) 0%,
            var(--beige-beam) calc(360deg / var(--amount-of-beams)),

            var(--yellow-beam) calc(360deg / var(--amount-of-beams)),
            var(--yellow-beam) calc(360deg / var(--amount-of-beams) * 2)
        );
    }
    .sun {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        background-color: #FAB12F;
    }
</style>