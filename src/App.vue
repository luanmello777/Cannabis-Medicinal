<template>
  <v-app>
    <v-app-bar color="#1B5E20">
      <div class="d-flex align-center justify-space-between w-100">
        <v-img src="../src/assets/images/logomed.jpg" :class="smAndDown ? ' w-0 h-0 pl-0 pr-0' : 'ml-5'" width="45"
          height="50"></v-img>

        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>


        <v-chip :class="smAndDown ? 'w-100 text-center justify-center ml-2' : 'mr-10'"
          class="chipcannabis  elevation-10 text-h5" size="x-large">
          <v-app-bar-title class="ml-10 mr-10">
            <div :class="smAndDown ? 'pl-16 pr-16' : 'text-h5'">
              <span class="font">Cannabis
                <svg-icon color="#C6FF00" type="mdi" :path="path"></svg-icon>
                Medicinal</span>
            </div>
          </v-app-bar-title>
        </v-chip>

        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>



        <v-dialog width="500">
          <template v-slot:activator="{ props }">
            <v-btn :class="smAndDown ? 'mr-2 ' : 'mr-10'"
              class="border rounded-xl elevation-10 ml-10 bg-lime-accent-3" v-bind="props"><svg-icon type="mdi"
                :path="path5"></svg-icon></v-btn>
          </template>

          <template v-slot:default="{ isActive }">
            <v-card title="Site de referência:" color="#1B5E20"
              :style="{ 'background-image': 'url(\'fundo.jpg\')', 'background-size': 'cover' }">
              <div class="text-center mt-5">
                <v-btn color="#C6FF00" href="https://www.cannabisativa.info/" target="_blank"><svg-icon type="mdi"
                    :path="path3" class="mr-3"></svg-icon>CANNABISATIVA.INFO</v-btn>
              </div>

              <div class="text-center mt-5">
                <v-btn color="#C6FF00" href="https://www.instagram.com/cannabisativa.info/" target="_blank"><svg-icon
                    type="mdi" :path="path4" class="mr-3"></svg-icon>CANNABISATIVA.INFO
                </v-btn>
              </div>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-dialog>
      </div>
    </v-app-bar>


    <v-main>


      <v-img src="../public/plant2.jpg" cover class="background-image">


        <v-container class="bg-green-darken-4 mt-10 pt-5 elevation-24 border rounded-xl">

          <v-carousel height="560" cycle hide-delimiter-background :show-arrows="false" color="#C6FF00" class="rounded">

            <v-carousel-item src="foto1.jpg" cover></v-carousel-item>

            <v-carousel-item src="foto2.jpg" cover></v-carousel-item>

            <v-carousel-item src="foto3.jpg" cover></v-carousel-item>

            <v-carousel-item src="foto4.jpg" cover></v-carousel-item>

          </v-carousel>


          <br>

          <div>

            <h2 class="font1 d-flex align-center justify-center w-45 border rounded-xl bg-black">QUANDO SURGIU?</h2>

            <br>
            <h3 class="text-black">
              Historicamente, há registros de indicações terapêuticas da Cannabis na China e no Egito antigo, que datam
              de
              4.000 a.C., assim como na medicina do subcontinente indiano e na Europa entre 2.000 e 1.000 a.C. Ainda antes
              de Cristo, o uso medicinal da Cannabis foi vastamente difundido pela cultura Greco-Romana para epilepsia,
              raiva, ansiedade, inflamações, dores de dente e de cabeça, e bronquite.
              Já em 1844, O'Shaughnessy retornou à Inglaterra, quando introduziu a cannabis na medicina ocidental
              e na
              farmacopeia do Reino Unido e posteriormente nos Estados Unidos, país que a adotou como medicação sedativa e
              anticonvulsivante, sob forma de extrato.
            </h3>
            <br>
            <br>

            <h2 class="font1 d-flex align-center justify-center w-45 border rounded-xl bg-black">C A N A B I N Ó I D E S
            </h2>

            <div class="ma-7 pb-5 d-flex justify-space-between" :class="smAndDown ? 'ml-0 mr-0  pb-3' : ''">
              <div style="width: 100px; height: 100px" class="elevation-15" :class="smAndDown ? '' : ''">
                <v-img src="../src/assets/images/one.jpg" alt="buddie de cannabis" width="300" height="300"
                  class="rounded"></v-img>

                <v-dialog width="500">
                  <template v-slot:activator="{ props }">
                    <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="THC"> </v-btn>
                  </template>

                  <template v-slot:default="{ isActive }">
                    <v-card title="THC">
                      <v-card-text>
                        O THC (tetrahidrocanabinol), como é conhecida a molécula mais psicoativa da cannabis, atua como
                        relaxante muscular e
                        anti-inflamatório. Dentre os benefícios, produz efeito anticonvulsivo, anti-inflamatório,
                        antidepressivo e anti-hipertensivo. Além de ser usado também como analgésico e no tratamento
                        para
                        aumentar o apetite.
                      </v-card-text>

                      <v-card-actions>
                        <v-spacer></v-spacer>

                        <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                      </v-card-actions>
                    </v-card>
                  </template>
                </v-dialog>

              </div>
              <div style="width: 100px; height: 100px" class="elevation-15" :class="smAndDown ? '' : ''" >
                <v-img src="../src/assets/images/two.png" alt="buddie de cannabis" width="300" height="300"
                  class="rounded"></v-img>

                <v-dialog width="500">
                  <template v-slot:activator="{ props }">
                    <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="CBD"> </v-btn>
                  </template>

                  <template v-slot:default="{ isActive }">
                    <v-card title="CBD">
                      <v-card-text>
                        O canabidiol, conhecido popularmente como CBD tem efeitos calmantes no sistema nervoso central.
                        Além disso, por não ter efeito narcótico, pode
                        substituir
                        os
                        ansiolíticos, que são viciantes. Devido as suas substâncias calmantes, o canabidiol auxilia no
                        tratamento da ansiedade, do sono, combate tumores, convulsões e reduz efeito psicotomimético do
                        THC, tornando assim uma substância com enorme potencial terapêutico.
                      </v-card-text>

                      <v-card-actions>
                        <v-spacer></v-spacer>

                        <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                      </v-card-actions>
                    </v-card>
                  </template>
                </v-dialog>
              </div>
              <div style="width: 100px; height: 100px" class="elevation-15" :class="smAndDown ? '' : ''">
                <v-img src="../src/assets/images/three.jpg" alt="buddie de cannabis" width="300" height="300"
                  class="rounded"></v-img>

                <v-dialog width="500">
                  <template v-slot:activator="{ props }">
                    <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="CBG"> </v-btn>
                  </template>

                  <template v-slot:default="{ isActive }">
                    <v-card title="CBG">
                      <v-card-text>
                        O CBG (canabigerol), é considerado o precursor de outros canabinóides. Isso ocorre porque o
                        CBG-A, a forma
                        ácida do
                        CBG, se decompõe para formar CBG, CBD, THC e CBC (canabicromeno, outro canabinóide) quando
                        aquecido.
                        CBD e CBG são ambos canabinóides não-psicoativos, o que significa que não o farão ficar
                        “chapado”.
                        Ambos também interagem com os mesmos receptores no corpo, de acordo com um estudo de 2018
                        (Trusted
                        Source) e parecem ter efeitos anti-inflamatórios. No entanto, o CBG parece ter algumas funções e
                        benefícios à saúde diferentes do CBD.
                      </v-card-text>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                      </v-card-actions>
                    </v-card>
                  </template>
                </v-dialog>

              </div>
            </div>

          </div>
        </v-container>

        <br>

        <v-container class="text-white mt-10 pt-5 elevation-24 border rounded-xl"
          :style="{ 'background-image': 'url(\'plant1.jpg\')', 'background-size': 'cover' }">
          <h2 class="font1 d-flex align-center justify-center w-45 border rounded-xl bg-black">ESPÉCIES DE CANNABIS</h2>
          <br>


          <div class="ma-7 pb-3 d-flex justify-space-between" :class="smAndDown ? 'mr-auto ml-auto pb-3' : ''">
            <div style="width: 100px; height: 100px" class="elevation-15">
              <v-img src="../public/four.png" alt="buddie de cannabis" width="100" height="100" class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="SATIVA"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Sativa">
                    <v-card-text>
                      <v-list>
                        <v-list-item v-for="(item, index) in items" :key="index">
                          <v-icon class="mr-2" color="#AEEA00">mdi-check-circle</v-icon>
                          {{ item }}
                        </v-list-item>
                      </v-list>
                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>

                      <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>

            </div>
            <div style="width: 100px; height: 100px" class="elevation-15">
              <v-img src="../public/five.png" alt="buddie de cannabis" width="100" height="100" class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="INDICA"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Indica">
                    <v-card-text>
                      <v-list>

                        <v-list-item v-for="(item, index) in items1" :key="index">
                          <v-icon class="mr-2" color="#AEEA00">mdi-check-circle</v-icon>
                          {{ item }}
                        </v-list-item>

                      </v-list>
                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>
            </div>
            <div style="width: 100px; height: 100px" class="elevation-15">
              <v-img src="../public/six.png" alt="buddie de cannabis" width="100" height="100" class="rounded"></v-img>


              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="RUDERALIS"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Ruderalis">
                    <v-card-text>

                      <v-list>
                        <v-list-item v-for="(item, index) in items2" :key="index">
                          <v-icon class="mr-2" color="#AEEA00">mdi-check-circle</v-icon>
                          {{ item }}
                        </v-list-item>
                      </v-list>

                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>
            </div>
          </div>
        </v-container>

        <br>

        <v-container class="bg-green-darken-4 mt-7 pt-5 elevation-24 border rounded-xl">

          <h2 :class="smAndDown ? 'text-h6-center pl-5' : ''"
            class="font1 d-flex align-center justify-center w-45 border rounded-xl bg-black">O PRECONCEITO ACABA ONDE A
            COMPREENSÃO COMEÇA</h2>

          <br>

          <h3 class="text-black">Por conta do seu potencial medicinal, mais de 35 países já regulamentaram o uso da
            cannabis para tratar pacientes com doenças graves ou raras, como epilepsia refratária, esclerose múltipla,
            ansiedade, autismo, dor crônica, Alzheimer, entre outras.
            O CBD, o THC, o CBG e o CBN são alguns dos canabinoides presentes na Cannabis com alto
            potencial terapêutico
            devido às suas propriedades anticonvulsivantes, anti-inflamatórias, ansiolíticas e antitumorais. <span
              class="text-lime-accent-3">
              Levantamos
              algumas das inúmeras patologias que podem ser tratadas com a cannabis </span> para você entender como a
            substância
            atua no organismo e seus benefícios à saúde.</h3>
          <br>

          <br>
          <div class="d-flex justify-space-between rounded">

            <v-img src="../public/med1.jpg" alt="médico e cannabis medicinal" width="150" height="125"
              class="rounded"></v-img>
            <v-img src="../public/med2.jpg" alt="médico e cannabis medicinal" width="150" height="125" class="rounded"
              :class="smAndDown ? 'w-0 h-0' : ''"></v-img>
            <v-img src="../public/med3.jpg" alt="médico e cannabis medicinal" width="150" height="125"
              class="rounded"></v-img>

          </div>
          <br>
        </v-container>
      </v-img>

      <HelloWorld />

    </v-main>
  </v-app>
</template>




<style>
.font {
  font-family: 'Young Serif', serif;
}


.font1 {
  font-family: 'Playfair Display', serif;
}
</style>







<script setup>
import HelloWorld from '@/HelloWorld.vue';
import { useDisplay } from 'vuetify';
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiCannabis, mdiCommentAccountOutline, mdiFileDocument, mdiInstagram, mdiViewHeadline } from '@mdi/js';

const { smAndDown } = useDisplay()

const path = mdiCannabis;
const path2 = mdiCommentAccountOutline;
const path3 = mdiFileDocument;
const path4 = mdiInstagram;
const path5 = mdiViewHeadline;
const items = [
  'Uso diurno, clareza e criatividade.',
  'Países de clima quente.',
  'Necessita de muita luz solar.',
  'Grande concentração de THC.',
  'Ideal para atividades físicas.',
];
const items1 = [
  'Uso noturno, relaxamento e reflexão.',
  'Clima ameno.',
  'Cresce menos.',
  'Possuem tanto CBD quanto THC.',
  'Redução do stress e da ansiedade.',
  'Ideal para dores e espasmos musculares.',
];
const items2 = [
  'Matéria-prima tradicional.',
  'Níveis muito baixos de THC e de CBD',
  'Sem efeitos medicinais',
  'Fonte de extração de cânhamo, fibra muito versátil usada para confeccao de tecidos, extração de combustível, papel ecológicos e até casas residenciais.'
];

</script>