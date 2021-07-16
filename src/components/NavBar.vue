<template>
  <div class="row px-5 box">
            
            <!-- logo -->
            <div class="col-4 p-4">
            <img src="../assets/images/logotype.png" alt="logo">
            </div>

            <!-- navbar -->
            <div class="col-8 px-4 text-end">
            <ul>
                <li v-for="(items,index) in navSuite" :key="index" class="mx-4"><a href="#">{{items}}</a></li>
            </ul>
            </div>

      </div>
</template>

<script>
export default {
    name: "NavBar",
    data(){
        return {
            navSuite: [
                "HOME",
                "ABOUT",
                "PROJECT",
                "SERVICE",
                "BLOG",
                "CONTACT"
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
header{
    .box{
        width: 100%;
       img {
        width: 112px;
        height: 19px;
        }
        ul{
            li{
                list-style: none;
                display: inline-block;
                padding-top: 40px;
            
                &:hover {
                    border-top: 3px solid white;
                    padding-top: 37px;
                    a{
                        font-weight: 800;      
                    }
            }
            a{
                color: $white_txt;
                text-decoration: none;
            }
        }
    } 
    }
    
}

</style>