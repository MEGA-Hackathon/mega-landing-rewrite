<template>
    <div id="home" class="home-page">
        <div>
            <h1>Empowering Thousands<br />With The Gift Of Technology</h1>
            <p>47 Countries Reached | $400k+ Raised & Awarded</p>
            <img class="home-image" :src="HomePageImage" alt="Home Page Image" />

            <div class="home-page-image">
            <img class="puzzle-image" :src="PuzzleImage" alt="Puzzle Image" />   
            <img class="circle-image" :src="CircularImage" alt="Circular Image"/>
            <img class="arrow-left" :src="ArrowLeft" alt="Arrow Image" />
            <img class="arrow-right" :src="ArrowRight" alt="Arrow Image" />
            <img class="message-image" :src="MessageImage" alt="Message Image" />
            </div>
            
        </div>
        </div>
</template>

<script>
import HomePageImage from '@/assets/banner-mockup.png';
import PuzzleImage from '@/assets/banner-icon-1-1.svg';
import MessageImage from '@/assets/banner-icon-1-2.svg';
import ArrowRight from '@/assets/banner-icon-1-3.svg';
import ArrowLeft from '@/assets/banner-icon-1-4.svg';
import CircularImage from '@/assets/banner-icon-1-6.svg'

export default {
    data () {
        return {
            HomePageImage,
            PuzzleImage,
            MessageImage,
            ArrowRight,
            ArrowLeft,
            CircularImage,
        };
    }
}
</script>

<style scoped>
.home-page {
    position: relative;
    margin-top: 50px;
}
.home-page h1 {
    font-size: 47px;
    font-weight: bold;
}

.home-page p {
    font-size: 22px;
}

.home-image {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 1.5rem;
    margin-left: 12rem;
    z-index: 2;
}

.puzzle-image {
    position: absolute;
    margin: 5rem 0 0 9rem;
    animation: moveSquare 7s linear infinite;
}

.message-image {
    position: absolute;
    margin: 5rem 0 0 70rem;
    animation: moveSquare 7s linear infinite;
}

.arrow-left {
    position: absolute;
    width: 25rem;
    height: 35rem;
    left: 0;
    margin: 10rem 0 0 -7rem;
    z-index: 1;
    animation: moveSquare 7s linear infinite;
}

.arrow-right {
    position: absolute;
    width: 25rem;
    height: 35rem;
    right: 0;
    margin: 10rem 0 0 65rem;
    z-index: 1;
    animation: moveSquare 7s linear infinite;
}

.circle-image {
    margin: 27rem 62rem 0 0;
    animation: rotate 7s linear infinite alternate;
}

@keyframes rotate {
    0% {
        transform: rotate(0);
    }
    100% {
        transform: rotate(90deg);
    }
}

@keyframes moveSquare {
    0% {
        top: 0;
        left: 0;
    }
    25% {
        top: 0;
        left: 20px;
    }
    50% {
        top: 20px;
        left: 20px;
    }
    75% {
        top: 20px;
        left: 20px;
    }
    100% {
        top: 0;
        left: 0;
    }
}

@media (max-width: 1024px){

    .home-page {
        margin-top: -10px;
    }

    .home-page h1 {
        font-size: 27px;
        width: 50%;
        margin-left: 12rem;
    }

    .home-page p {
        font-size: 20px;
    }

     .home-image {
       width: 80%;
       margin: 40px 0 0 5.5rem;
    }

    .home-page-image {
        visibility: hidden;
    }

}


@media (max-width: 760px) {
    .home-page {
        margin-top: -20px;
    }

    .home-page h1 {
        font-size: 27px;
        width: 100%;
        margin-left: 20px;
    }

    .home-page p {
        font-size: 17px;
        margin-left: 30px;
    }

    .home-image {
       width: 100%;
       margin: 40px 0 0 10px;
    }

    .home-page-image {
        visibility: hidden;
    }
}
</style>