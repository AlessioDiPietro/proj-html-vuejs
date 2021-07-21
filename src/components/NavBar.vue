<template>
<div class="container-fluid w-50 m-0 text-center">
  <div class="row box">

            <!-- navbar -->
            <div class="px-4">
            <ul class="p-0">
                <li v-for="(items,index) in navSuite" :key="index" class="mx-4"><a :href="'#'+items">{{items}}</a></li>
            </ul>
            </div>

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
    .box{
        width: 100%;
        ul{
            li{
                list-style: none;
                display: inline-block;
                padding-top: 40px;
                transition: all 1s linear;
            
                &:hover {
                    border-top: 3px solid white;
                    padding-top: 36px;  
               }
            }           
            a{
                color: $title_grey_txt;
                text-decoration: none;
                &:focus {
                    font-weight: 800;
                    color: $white_txt;
                }
            }
            
        }
    } 
    

</style>