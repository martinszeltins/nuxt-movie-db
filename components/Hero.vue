<template>
  <div class="hero">
    <img src="../assets/movieHero.jpg" />

    <div class="text-container">
      <div class="text">
        <span class="mini-heading">
            Now Stremaing
        </span>

        <h1>
            <span>Now</span> Streaming
        </h1>

        <a href="#movie-grid" class="button">
            View Movies
        </a>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: 'hero',
    }
</script>

<style scoped>
    .hero {
        height: 400px;
        position: relative;
    }
    @media (min-width: 750px) {
        .hero {
            height: 500px;
        }
    }
    .hero::after {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        background-color: rgba(0, 0, 0, 0.6);
    }
    .hero img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    .hero .text-container {
        z-index: 99;
        position: absolute;
        top: 0;
        margin: 0;
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .hero .text-container .text {
        padding: 0 16px;
        width: 100%;
        max-width: 1400px;
        margin: 0 auto;
    }
    .hero .text-container .mini-heading {
        font-weight: 600;
        font-size: 18px;
        text-transform: uppercase;
        color: #c92502;
        margin-bottom: 8px;
    }
    @media (min-width: 750px) {
        .hero .text-container .mini-heading {
            font-size: 22px;
        }
    }
    .hero .text-container h1 {
        color: #fff;
        font-size: 64px;
        font-weight: 200;
        margin-bottom: 8px;
    }
    @media (min-width: 750px) {
        .hero .text-container h1 {
            font-size: 84px;
        }
    }
    .hero .text-container h1 span {
        font-weight: 500;
    }
    .hero .text-container .button {
        font-size: 20px;
        align-self: flex-start;
    }
</style>