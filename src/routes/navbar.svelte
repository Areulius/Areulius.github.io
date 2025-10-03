<nav>
    <div class="container">
        <a href="/" class="icon">
            <img src="src\lib\assets\VA_Logo1.2.webp" alt="" class="logo-img" />
        </a>
        <div class="nav-links">
            <a href="/" class="link">Home</a>
            <a href="/about" class="link">About</a>
            <a href="/game" class="link">Game</a>
            <a href="/blocks" class="link">Blocks</a>
        </div>
    </div>
</nav>

<style>
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 80px;
    }

    .nav-links {
        margin: 10px 20px 10px 20px;
    }

    .link {
        margin: 5px 10px 5px 10px;
        color: black;
        font-size: 35px;
        font-weight: bolder;
    }


    .icon {
        --image-size: 60px;
        
        width: var(--image-size);
        height: var(--image-size);
        margin: 10px;
        border-radius: 50%;
    }
    .icon > img {
        height: var(--image-size);
        width: var(--image-size);
        border-radius: 50%;
    }
</style>