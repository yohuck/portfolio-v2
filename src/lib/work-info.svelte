<article class="portfolio-info">
    <div class="info">
        <input type="button" id="x" value="x">
        <div class="info-text">
            <h4>Scroll around out some of my recent work.</h4>
            <p>Want to see how they look on mobile? Click the 📱 and I'll text you a link.</p>
        </div>
        <form action="submit">
            <input type="tel">
            <input type="submit">
        </form>

    </div>
</article>

<style>
    .portfolio-info {
        height: 100vh;
        position: absolute;
        width: 100vw;
        color: black;
        z-index: 6;
        background-color: rgba(5, 10, 5, 0.836);
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        transform: scale(1);

    }

    .info{
        width: 70%;
        background-color: rgb(240, 255, 249);
        padding: 2rem;
        max-width: 500px;
        border-radius: 5px;
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        align-items: flex-end;

    }

    .info-text{
        width: 100%;
    }

    #x{
        width: 2rem;
        height: 2rem;
    }
</style>