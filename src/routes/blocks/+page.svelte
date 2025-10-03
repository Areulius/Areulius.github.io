<script>
    import Navbar from '../navbar.svelte'
</script>

<Navbar />

<div class="container">
    <h1 class="title">Welcome to Blocks</h1>
    <h4 class="title">This is a testing ground</h4>
</div>

<style>
    .container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-color: rgb(54, 138, 65);
        border-bottom: 6px solid rgb(12, 85, 37);
        border-radius: 10px;
    }

    .title {
        margin: 5px;
        color :bisque;
        font-family: OCR A Std, monospace;
    }
</style>