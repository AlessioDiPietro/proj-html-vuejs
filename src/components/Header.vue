<template>
  <header id="HOME">
      <div class="red_side position-relative">

        <div class="header_top d-flex justify-content-between">
            
            <img src="../assets/images/logotype.png" alt="logo" class="animlogo">
            <NavBar/>
          
        </div>



        <div class="promo position-absolute slide-top">
            <div class="green_line"></div>
            <span>ALWATS THE BEST WAY YOU NEED IT</span>
            <h1>THE BEST BUSINESS CONSULTING</h1>
            <button class="read_me">READ MORE</button>
            <button class="play_btn"><i class="fas fa-play"></i></button>
        </div>

      </div>

  </header>
</template>

<script>
import NavBar from "@/components/NavBar.vue"
export default {
    name:"Header",
    components: {
        NavBar
    },
    

}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
    .red_side {
        background-image: url("~@/assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg");
        background-repeat: no-repeat;
        background-position: right;
        height: 980px;
        .header_top{
            @include form_section_90;
            margin-top: 0;
        }
        .promo{
            width: 600px;
            left: 162px;
            top: 35%;
            font-size: 20px;
            .green_line {
                display: inline-block;
                height: 3px;
                width: 50px;
                margin-right: 20px;
                background-color: $opa_maringreen_bg;
            }
            h1 {
                font-size: 120px;
                font-weight:bolder;
            }
            .read_me {
                @include btn_maringreen;
                &:hover{
                    animation: colorbtn 1s ease 0s 1 normal forwards;
                    @keyframes colorbtn {
                        0% {
                            animation-timing-function: ease-in;
                            opacity: 0;
                            transform: scale(7);
                        }

                        38% {
                            animation-timing-function: ease-out;
                            opacity: 1;
                            transform: scale(1);
                        }

                        55% {
                            animation-timing-function: ease-in;
                            transform: scale(1.5);
                        }

                        72% {
                            animation-timing-function: ease-out;
                            transform: scale(1);
                        }

                        81% {
                            animation-timing-function: ease-in;
                            transform: scale(1.24);
                        }

                        89% {
                            animation-timing-function: ease-out;
                            transform: scale(1);
                        }

                        95% {
                            animation-timing-function: ease-in;
                            transform: scale(1.04);
                        }

                        100% {
                            animation-timing-function: ease-out;
                            transform: scale(1);
                            background-color: $int_red_bg;
                        }
                    }
                }
                
            }
            .play_btn {
                padding:15px 20px;
                margin: 0 30px;
                border-radius: 50%;
                background-color: transparent;
                border: 2px solid $int_maringreen_bg;
                color: $int_maringreen_bg;
                transition: all linear 2s;
                &:focus{
                    border: 2px solid $int_red_bg;
                    color: $int_red_bg;
                }
            }
        }
    }
    img {
        width: 112px;
        height: 19px;
        margin-top: 43px;
    }

    .slide-top {
	-webkit-animation: slide-top 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
	animation: slide-top 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
}

@-webkit-keyframes slide-top {
  0% {
    -webkit-transform: translateY(0);
            transform: translateY(0);
  }
  100% {
    -webkit-transform: translateY(-100px);
            transform: translateY(-100px);
  }
}
@keyframes slide-top {
  0% {
    -webkit-transform: translateY(0);
            transform: translateY(0);
  }
  100% {
    -webkit-transform: translateY(-100px);
            transform: translateY(-100px);
  }
}

    



</style>