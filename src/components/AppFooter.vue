<script >
export default {
    name: "footer"
}
</script>


<template>
    <div class="full-section">

        <div class="contenitore">
            <div class="main-footer">
                <div class="links">
                    <div class="col-3">
                        <ul>
                            <li class="title"> titolo</li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>

                        </ul>
                        <ul>
                            <li class="title"> titolo</li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>

                        </ul>
                    </div>
                    <div class="col-3">

                        <ul>
                            <li class="title"> titolo</li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                        </ul>
                    </div>
                    <div class="col-3">
                        <ul>
                            <li class="title"> titolo</li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                            <li> <a>contenuto</a></li>
                        </ul>

                    </div>

                </div>
                <img class="img-dc" src="/img/dc-logo-bg.png" alt="img">
            </div>
        </div>
    </div>
    <div class="social-section">
        <div class="contenitore">

            <button>Sign-Up Now</button>
            <div class="socials">
                <h4><a href="#">FOLLOW US</a></h4>
                <div class="logos">
                    <img src="/img/footer-facebook.png" alt="fb">
                    <img src="/img/footer-twitter.png" alt="fb">
                    <img src="/img/footer-youtube.png" alt="fb">
                    <img src="/img/footer-periscope.png" alt="fb">
                    <img src="/img/footer-pinterest.png" alt="fb">
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use "../assets/scss/variables" as *;
@use "../assets/scss/partials" as *;


.img-dc {
    height: 580px;
    position: relative;
    top: -60%;

}

.full-section {
    padding: 50px 0;
    background-image: url("./img/footer-bg.jpg");
    background-size: cover;
    height: 400px;
    overflow: hidden
}

.contenitore {
    @include contenitore;



}

.col-3 {
    width: 30%;
}



.links {
    width: 40%;
    display: flex;


}

ul {



    width: 100px;

    li {
        color: white;

        list-style-type: none;

        &.title {
            font-size: 25px;
            font-weight: bold;
            margin: 6px 0;

        }

    }

}


.main-footer {
    display: flex;
    justify-content: space-between;
    height: 200px;
}


.social-section {
    background-color: #303030;

    .contenitore {
        height: 130px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .socials {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        a {
            text-decoration: none;
            color: #077AE5;
            font-size: 20px;
        }

        .logos {
            height: 30px;
            display: flex;
            justify-content: space-between;
            margin-left: 25px;
            width: 200px;

            img {
                height: 100%;
            }
        }
    }
}

button {
    background-color: #303030;
    font-size: 17px;
    font-weight: bold;
    padding: 20px 10px;
    border-color: #077AE5;
    color: white;

}
</style>