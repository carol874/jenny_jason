<script setup>
import { ref } from 'vue';

const abrirMenu = ref(false);



</script>

<template>
  <header class="cabeca">
    <nav class="topo">
      <div class="um">
       <h1>J&J</h1>
      <h3>JUNE 23RD,2025</h3>
      </div>
      <button @click="abrirMenu = !abrirMenu" class="hamburguer">
        ☰
      </button>
      <div class="dois" :class="{ ativo: abrirMenu }">
        <li>
          <a href="">HOME</a>
        </li>
        <li>
          <a href="">OUR STORY</a>
        </li>
        <li>
          <a href="">DETAILS</a>
        </li>
        <li>
          <a href="">RSVP</a>
        </li>
      </div>
      
    </nav>
  </header>

  <main>
    <h1 class="titulo">
      JENNY & JASON
    </h1>
    <section class="meio">
      <img src="./assets/tomoko-uji-kxvn1ogpTtE-unsplash.jpg" alt="">
      <p>
      
With love and gratitude, we invite you to share in the joy of our wedding day.
Saturday, September 20, 2025.
The Golden Elm Manor, St. Augustine, New York.
      </p>
    </section>

    <section class="imagens">
      <div class="flor">
        
             <img src="./assets/amber-kipp-1hRtZo55-DE-unsplash.jpg" alt="">
             <p>
              HOME
             </p>
        </div>

        <div class="flor">
            <img src="./assets/tirza-van-dijk-cNGUw-CEsp0-unsplash.jpg" alt="">
            <p>
              THE DETAILS
            </p>
        
        </div>

        <div class="flor">
     
            <img src="./assets/mina-rad-8fS2YgV1cBs-unsplash.jpg" alt="">
            <p>
              RSVP
            </p>
          </div>


        <div class="flor">
            <img src="./assets/sidney-pearce-yPMJliKzyc4-unsplash.jpg" alt="">
            <p>
              REGISTRY
            </p>
      </div>

    </section>

    <section class="quase">
      <div>
        <img src="./assets/coisa.jpg" alt="">
      </div>
      <div class="registro">
        <h1>RESGISTRY</h1>
      </div>

      <div class="presenca">
    <p>
Your presence is the most cherished gift. Should you wish to contribute, we’ve created a honeymoon registry to help us embark on a memorable adventure to the Amalfi Coast.
</p>

      </div>

      <div class="botao">
        <p>GO TO REGISTRY</p>
      </div>
      
    </section>


    <section class="presentes">
        <div class="img">
          <img src="./assets/simona-sergi-9AosJc43_nQ-unsplash (1).jpg" alt="">
        </div>
        <div class="texto">
     <h1>
      PRESENT IDEAS
     </h1>
        </div>
      
    </section>
  </main>
  <footer>
    <div>
      <p>J&J</p>
    </div>
    <div>
      <p>
        SATURDAY, <br>
        SEPTEMBER 20,2025
      </p>
    </div>
  </footer>
  
</template>

<style scoped>
.cabeca{
 background-color: #939393;
 border-radius: 20px;
 
}
.topo{
   font-family: "Playfair Display SC", serif;
   display: flex;
  justify-content: space-between; 
  align-items: center;
  color: white;
}
.topo li a{
  color: white;
 
}

.titulo{
  text-align: center;
  font-size: 5rem;
  font-family: "Playfair Display SC", serif;
  font-weight: 300;
  padding: 2vw;
}
.dois{
   font-size: 0.9rem;
   display: flex;
  gap: 30px; 
  list-style: none;
  margin-right: 20px; 
  
}
.um{
  display: flex;
  
}
.um h1{
  padding: 1vw;
  font-weight: 400;
}
.um h3{
  font-size: 0.9rem;
  padding: 2.2vw;
  font-weight: 400;
}
.meio p{
  font-family:"Playfair Display SC", serif ;
  text-align: center;
  font-size: 2rem;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.meio{
  position: relative;
 
}
.meio img{
  width: 100%;
  object-fit: cover;
}
.imagens{
  display: grid;
 grid-template-columns: repeat(2, 350px);
  gap: 5.6vw;
  padding: 3vw;
  justify-content: center;
  padding: 7vw 0 0 0;
}

.flor{
  position: relative;
  
}

.flor img{
  width: 100%;
  border-radius: 2vw;
  
}

.flor p{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  font-size: 1.8rem;
  font-family: "Playfair Display SC", serif;
  text-decoration: underline;
}

.botao p{
  background-color: #939393;
  padding: 1.2vw;
  font-family:"Playfair Display SC", serif ;
  color: white;
  text-align: center;
  border-radius: 15px;
  position: absolute;
  top: 90%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 1.2rem;
  
}
.registro{
  text-align: center;
  font-family:"Playfair Display SC", serif ;
  font-size: 2rem;
  position: absolute;
  top: 35%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  
}
.presenca{
  text-align: center;
  font-family:"Playfair Display SC", serif ;
  font-size: 1.6rem;
  position: absolute;
  top: 65%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}
.quase div img{
  width: 100%;
  
}
.quase img{
  object-fit: cover;
}
.quase {
  padding: 10vw 0 0 0;
  position: relative;
}

.img img{
  width: 100%;
}
.presentes{
  position: relative;
  padding: 20vw 0 13vw 0;
}
.presentes .img img{
   object-fit: cover;
}
.texto{
  text-align: center;
  font-family:"Playfair Display SC", serif ;
  color: white;
  top: 45%;
  left: 50%;
   transform: translate(-50%, -50%);
   position: absolute;
   font-size: 1.6vw;
   text-decoration: underline;
   
}
footer{
  background-color: #EDE0E0;
  padding: 1vw;
}
footer div p{
  text-align: center;
  font-family: "Aboreto", system-ui;
  font-weight: 200;
  font-style: normal;
  font-size: 2rem;
}
.hamburguer {
  display: none;
  font-size: 24px;
  background: none;
  border: none;
  color: white;
  cursor: pointer;
}
@media (max-width: 600px){
  .hamburguer {
    display: block;
  }

  .dois {
    position: absolute;
    top: 30px;
    right: 0;
    background-color: #939393;
    flex-direction: column;
    padding: 18px;
    z-index: 99;
    border-radius: 0px 0px 16px 16px;
    gap: 13px;
    li a {
      font-size: 17px;
    }
  }
    .dois{
    display: none;
  }

  .dois.ativo{
    display: flex;
  }
 .titulo{
  font-size: 3rem;
  text-align: center;
 }
.meio p{
 font-size: 1.2rem;
  line-height: 1.2;
  width: 80%;
  padding: 0 0 7vw 0 ;
  margin: 2vw;
}
.meio img{
  height: 40vh;
}
.imagens{
   grid-template-columns: 1fr;
  justify-items: center;
  
}
.flor{
  width: 80%;
}

.flor img{
  width: 100%;
}
.cabeca {
  .topo {
    padding-inline: 5vw;
    .um {
      h1 {
        font-size: 5vw;
      }
      h3 {
        font-size: 2vw;

      }
    }
  }
}


.presentes .img img{
  height: 35vh;
}
.presentes .texto h1{
  font-size: 1.5rem;
}
footer div p{
  font-size: 1.5rem;
}
footer{
  padding: 6vw;
}
.quase  img{
 height: 40vh;
}
.quase .presenca{
  width: 97%;
  font-size: 1rem;
  line-height: 1.1;
}
.quase .presenca p{
  margin: 0;
}

.quase .botao p {
  font-size: 0.9rem;
  padding: 0.3rem;
}
.quase .registro h1{
   font-size: 2.1rem;
              
}
}
</style>
