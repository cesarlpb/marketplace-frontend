<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HomeView from './views/HomeView.vue'
</script>

<template>
 
<router-view></router-view>

</template>

<style scoped>
*{
    box-sizing: border-box;
}

html{
    scroll-behavior: smooth;
}

body{
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    margin: 0;
    background-color:rgba(45, 82, 182, 0.253)
}

h1{ font-size: 3.7em;}
h2{ font-size: 2.7em;}
h3{ font-size: 2em;}
p{ font-size: 1.25;}
ul{ list-style: none;}
li{font-size: 1.25em;}

button{
    font-size: 1.5em;
    font-weight: bold;
    padding: 10px 30px;
    border-radius: 10px;
    border: 1px solid rgba(0,0,0,0.5);
    box-shadow: 2px 2px 10px rgba(0,0,0,0.5);
    color: white;
    background-color: rgba(0, 0, 0, 0.63);
}

button:hover{
    background-color: rgb(63, 24, 100);
}

.container{
    max-width: 1400px;
    margin: auto;
}

.color-acento {color: aqua;}

header{
    background-color: rgba(233, 225, 215, 0.596);
}

header .logo{
    margin: 0;
    padding: 25px 30px;
    font-weight: bold;
    color: blueviolet;
    font-size: 1.65em;
}

header .container{
    display: flex;
    flex-direction: column;
    align-items: center;
}

header nav{
    display: flex;
    flex-direction: column;
    text-align: center;
    padding-bottom: 25px;
}

header a{
    padding: 5px 12px;
    text-decoration: none;
    font-weight: bold;
    color: black;
}

header a:hover{
    color: blueviolet;
}

#hero{
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    height: 90vh;
    color: black;
    background-image: url("media/Recurso1.png");
    background-size: cover;
    background-repeat: no-repeat
    
}

#hero h1{
    color: rgb(255, 255, 255);
    margin-top: -15%;
}

#hero button{
    font-size: 1.75em;
}

#descripcion .container{
    text-align: center;
    padding: 200px 12px;

}

#nuestros-programas{
    background-color: rgba(24, 23, 23, 0.877);
    color: rgb(255, 255, 255);
    text-align: center;
}

#nuestros-programas .container{
    padding:  100px 0px;
}
#nuestros-programas h2{
    margin-top: 0%;
    font-size: 3em;
}

#nuestros-programas p{
    display: none;

}

#nuestros-programas .carta{
    background-position: center center;
    background-size: cover;
    padding: 50px;
    margin: 20px;
    border-radius: 15px;
}

.carta:first-child{
    background-image: url("media/webdesign.jpg");
    
    
    
}

.carta:nth-child(2){
    background-image: url("media/appweb.jpg");
    
}

.carta:nth-child(3){
    background-image: url("media/ecommerce.jpg");
    
}

#caracteristicas .container{
    text-align: center;
    padding: 200px 12px;
}
#caracteristicas li{
    margin: 15px 0px;
    font-weight: bold;
}

#final{
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    height: 80vh;
    background-color: rgb(30,30,30);
    color: white;
}

#final h2{
    font-size: 9vw;
}

#final button{
    font-size: 5vw;
}

footer{
    background-color: rgb(105, 101, 101);
}

footer p{
    margin: 0;
    padding: 12px;
    color: rgb(248, 245, 245);
}

footer .container{
    height: 150px;
    justify-content: center;
    align-items: flex-end;
    display: flex

}

@media (min-width: 720px){
    header{
        position: fixed;
        width: 100%;
    }
    header .container{
        flex-direction: row;
        justify-content: space-between;
    }

    header nav{
        flex-direction: row;
        padding-bottom: 0;
        padding-right: 20px;
    }

    #hero h1{
        font-size: 6.5em;
        
    }

    #descripcion .container{
        display: flex;
        justify-content: space-evenly;
    }

    #descripcion .texto{
        width: 50%;
        max-width: 600px;
        text-align: initial;
        padding-left: 50px;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    
    #descripcion h2{
        margin-top: 0px;
    }

    #descripcion .img-container{
        background-image: url("media/banner.jpg");
        background-size: cover;
        background-position: center center;
        height: 400px;
        width: 1000px;
    }

    #nuestros-programas .programas{
        display: flex;
        justify-content: center;
    }

    #nuestros-programas p{
        display: block;
        margin-bottom: 30px;
    }

    #nuestros-programas h3{
        margin-top: 0;
    }

    #nuestros-programas .carta{
        padding: 50px;
    }

    #caracteristicas{
        background-image: url("media/desarrollo.webp");
        background-repeat: no-repeat;
        background-size: 900px 590px;
    }
    

    #caracteristicas .container{
        text-align: flex-end

    }

    #caracteristicas ul{
        margin-left: 100px;
    }


}
</style>
