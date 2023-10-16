
<template>
  <v-img src="../public/plant2.jpg" cover class="background-image">
    <v-main>



      <v-container class="pt-5 elevation-24 border rounded-xl"
        :style="{ 'background-image': 'url(\'plant2.jpg\')', 'background-size': 'cover' }">

        <h2 class="font1 d-flex align-center justify-center text-white bg-black border rounded-xl"
          :class="smAndDown ? 'pl-5' : ''">PATOLOGIAS TRATADAS COM A CANNABIS
        </h2>

        <br>

        
          <div class="ma-7 d-flex justify-space-between" :class="smAndDown ? 'mr-auto ml-auto pb-3' : ''">
            <div style="width: 100px; height: 100px" class="elevation-15">
              <v-img src="../public/cancer.png" alt="cancer" width="100" height="100" class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="CÂNCER"></v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Câncer de Mama">
                    <v-card-text>
                      Cada vez mais pacientes com câncer estão recorrendo à cannabis para auxílio terapêutico. Segundo
                      uma
                      pesquisa norte-americana publicada no Journal of Clinical Oncology (2020), de 725 pacientes com
                      câncer
                      de mama, 42% se trataram com cannabis como terapia auxiliar, buscando combater os efeitos
                      colaterais
                      da quimioterapia, como dores, náuseas e inapetência. Além disso, 57% usam a cannabis para tratar
                      ansiedade, 51% para diminuir o estresse e 70% para afastar a insônia, sintomas comuns
                      decorrentes da
                      doença. Há relatos de diminuição significativa no tamanho de tumores e estudos comprobatórios.

                      <h3>Link do artigo:</h3>
                      <a href="https://wecann.academy/br/cannabis-e-cancer-de-mama//"
                        target="_blank">WeCann.Academy/cannabis-e-cancer</a>
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
              <v-img src="../public/autismo.png" alt="autismo" width="100" height="100" class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="AUTISMO"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Autismo">
                    <v-card-text>
                      Por conta de inúmeros casos de sucesso, muitos pais de filhos autistas encontram na cannabis
                      medicinal
                      o tratamento de maior impacto na qualidade de vida do paciente e da família. O principal avanço
                      percebido na vida dessas pessoas é na melhora da interação social, além da insônia e o
                      Transtorno do
                      Déficit de Atenção com Hiperatividade, diminuindo crises e estabilizando o humor.
                      Pesquisa realizada por cientistas do Departamento de Ciências Fisiológicas do Instituto de
                      Ciências
                      Biológicas da Universidade de Brasília e médicos da Associação Brasileira de Pacientes de
                      Cannabis
                      Medicinal (Ama+me) durante os anos de 2016 e 2017 foi pautada nas impressões dos pais sobre a
                      mudança
                      no comportamento de seus filhos após a adoção da terapia canabinoide. Como resultado 78%
                      apresentaram
                      melhoras nos principais sintomas relacionados ao autismo.

                      <h3>Link do artigo:</h3>
                      <a href="https://unbciencia.unb.br/biologicas/104-ciencias-biologicas/637-estudo-aponta-beneficios-no-uso-de-cannabis-em-tratamento-com-autistas"
                        target="_blank">UnbCiencia/estudo-autista-cannabis</a>
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
              <v-img src="../public/depressao.png" alt="buddie de cannabis" width="100" height="100"
                class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="DEPRESSÃO"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Ansiedade, depressão e burnout">
                    <v-card-text>
                      Segundo a pesquisa realizada pelo Hospital das Clínicas (USP), a cannabis pode melhorar em cerca
                      de
                      60% dos sintomas de ansiedade, depressão e burnout. Por conta da rápida ação dos
                      fitocanabinoides,
                      há
                      uma melhora na saúde mental do paciente já nas primeiras semanas.
                      Os resultados apontam redução de 60% dos sintomas de ansiedade, 50% da depressão e 25% de
                      burnout
                      entre os voluntários que fizeram o tratamento padrão com canabidiol quando comparado com aqueles
                      que
                      só fizeram o tratamento padrão.

                      <h3>Link da pesquisa:</h3>
                      <a href="https://www.fmrp.usp.br/pb/arquivos/8337" target="_blank">Usp/cannabis-tratamento</a>
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
        
           <br>
      
          <div class="ma-7 d-flex justify-space-between" :class="smAndDown ? 'mr-auto ml-auto pb-3' : ''">
            <div style="width: 100px; height: 100px" class="elevation-15">
              <v-img src="../public/alzheimer.jpg" alt="buddie de cannabis" width="100" height="100"
                class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="ALZHEIMER"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Alzheimer">
                    <v-card-text>
                      Os efeitos positivos do tratamento da Doença de Alzheimer pela cannabis estão relacionados com o
                      sistema endocanabinoide, evitando o estresse oxidativo, a neuroinflamação e os danos neurais. De
                      certo
                      modo, a cannabis age prevenindo ou retardando a sua progressão, objetivo que nenhum outro
                      medicamento
                      atinge.

                      <h3>Baixe o arquivo:</h3>
                      <a href="https://rsdjournal.org/index.php/rsd/article/download/6073/5023&hl=pt-BR&sa=X&ei=Qz3YYbKKJ8vFywT297WADg&scisig=AAGBfm22vctw7qygE2kozlPA9eoTwjlcDQ&oi=scholarr"
                        target="_blank">Baixar Artigo Alzheimer</a>
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
              <v-img src="../public/fibromialgia.jpg" alt="buddie de cannabis" width="100" height="100"
                class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="DORES"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Fibromialgia e Dores crônicas">
                    <v-card-text>
                      Atualmente o tratamento da fibromialgia é constituído por grupo alopático que inclui relaxante
                      muscular, analgésicos e opioides, antidepressivos e anticonvulsivantes. Essa medicação é de alto
                      custo
                      e produz diversos efeitos colaterais, como boca seca e sonolência, afetando diretamente no
                      aspecto
                      social do paciente, diminuindo suas interações. Com a cannabis, diversos estudos apresentados
                      relataram diminuição de dor e melhora da qualidade de vida, com poucos efeitos colaterais e mais
                      assertivo com os sintomas.
                      Pesquisa desenvolvida por cientistas do campus de Ribeirão Preto da USP em animais de
                      laboratório
                      mostra a ação positiva do CBD na redução da dor crônica e comorbidades associadas, como
                      ansiedade. A
                      pesquisadora Gleice K. Silva-Cardoso, do Programa de Pós-Graduação em Psicobiologia da Faculdade
                      de
                      Filosofia, Ciências e Letras de Ribeirão Preto (FFCLRP) da USP, acredita que o CBD seja uma
                      estratégia
                      promissora no tratamento da dor crônica neuropática já que o sistema canabinoide tem
                      participação
                      essencial no circuito de sensibilidade à dor.

                      <h3>Link do artigo:</h3>
                      <a href="http://fait.revista.inf.br/imagens_arquivos/arquivos_destaque/SjdBMHOxDSuOA3x_2020-9-1-19-54-43.pdf"
                        target="_blank">Fait-Dores-cronicas</a>
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
              <v-img src="../public/parkinson.png" alt="buddie de cannabis" width="100" height="100"
                class="rounded"></v-img>

              <v-dialog width="500">
                <template v-slot:activator="{ props }">
                  <v-btn color="#C6FF00" width="300" class="mt-2" v-bind="props" text="PARKINSON"> </v-btn>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card title="Parkinson">
                    <v-card-text>
                      Pacientes com doença de Parkinson (DP) em uso de cannabis medicinal declaram ter percepções de
                      melhora
                      nos sintomas parkinsonianos. Mais de 1 mil pessoas responderam a um questionário e os resultados
                      são
                      bem expressivos, onde 40% afirmaram sentir redução da dor e cãibras musculares ao incluir a
                      planta
                      no
                      tratamento, 20% apresentaram melhora em relação à rigidez, freezing – “congelamento”, tremores,
                      depressão, ansiedade e síndrome das pernas inquietas. De forma geral, 54% das pessoas que
                      utilizaram
                      o
                      CBD via oral relataram melhoras, assim como, 68% das que inalaram Cannabis contendo THC.

                      <h3>Link do artigo:</h3>
                      <a href="https://wecann.academy/cannabis-e-parkinson/"
                        target="_blank">WeCann.Academy/cannabis-e-parkinson</a>
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
          <br>
      </v-container>

      <v-container class="bg-green-darken-4 mt-12 pt-5 elevation-24 border rounded-xl">

        <h2 class="font1 d-flex align-center justify-center border rounded-xl bg-black" :class="smAndDown ? 'pl-5' : ''">
          COMO TER ACESSO AO TRATAMENTO ?
        </h2>
        <br>
        <h3 class="text-black">
          O acesso ao tratamento com cannabis pode parecer bastante complicado e burocrático, porém graças aos avanços
          recentes de nossa legislação e da Anvisa se tratar com cannabis já é realidade para muitos brasileiros. Veremos
          a
          seguir o passo a passo de como iniciar o tratamento de forma segura e de acordo com as leis vigentes.
        </h3>
        <br>
        <h2 class="font1 d-flex align-center justify-center border rounded-xl bg-black">ETAPAS PARA O ACESSO</h2>
        <br>
        <h2 class="font1">CONSULTA MÉDICA :</h2>
        <h3 class="text-black">O primeiro passo para ter acesso ao tratamento com cannabis é a consulta médica. Pela
          resolução RDC n°3, de 23 de janeiro de 2015, a Anvisa passou a considerar os cannabinoides presentes na planta
          como substâncias medicinais, diante disso todo médico fica autorizado a prescrever medicamentos à base de
          cannabis
          para seus pacientes. Entretanto, os médicos também devem procurar se qualificar e aprender mais sobre o sistema
          endocanabinoide, pois só assim terá embasamento suficiente para oferecer o melhor tratamento.
          Atualmente, para prescrever qualquer medicação à base de cannabis o médico precisa apenas fornecer a receita
          médica contendo nome do paciente, nome comercial do produto, posologia, data, assinatura e número do registro no
          conselho de classe do médico (CRM).
        </h3>
        <br>
        <v-btn color="#C6FF00" href="https://amame.org.br/lista-de-prescritores-de-cannabis/" target="_blank"
          class=" d-flex align-center justify-center">LISTA DE PRESCRITORES
            DE CANNABIS</v-btn>
        <br>

        <h2 class="font1">AUTORIZAÇÃO DA ANVISA :</h2>
        <h3 class="text-black">Após obter a receita médica, é necessário solicitar junto à Anvisa a autorização para poder
          importar a medicação de cannabis. A autorização é válida por 2 anos e durante este tempo os pacientes ou seus
          representantes legais podem importar o produto autorizado.
          A autorização pode ser feita diretamente no site da ANVISA, <span class="text-white">clique no link abaixo
            para ser redirecionado</span>.</h3>
        <br>
        <v-btn color="#C6FF00"
          href="https://www.gov.br/pt-br/servicos/solicitar-autorizacao-para-importacao-excepcional-de-produtos-a-base-de-canabidiol"
          target="_blank" class=" d-flex align-center justify-center">
          AUTORIZAÇÃO
          PARA IMPORTAÇÃO</v-btn>
        <br>
        <h2 class="font1" :class="smAndDown ? 'ml-1' : ''">ACOMPANHAMENTO MÉDICO :</h2>
        <h3 class="text-black">O tratamento com cannabis medicinal deve ser constante e sempre seguido de acompanhamento
          médico. Como todo tratamento, cada pessoa tem o seu próprio tempo para reagir à medicação, enquanto algumas já
          sentem os benefícios nos primeiros dias, outras pessoas podem sentir melhorias a partir do segundo mês. Além
          disso, existe uma variedade enorme de genéticas de cannabis, onde cada uma possui benefícios específicos para
          cada
          patologia tratada.
          É através do acompanhamento médico que se pode chegar à melhor medicação para o paciente. O elevado aumento no
          número de pacientes que encontram resultados nesse tratamento fez com que a classe médica buscasse se capacitar
          sobre a medicina canabinoide, aumentando em 554% no número de prescritores de cannabis medicinal entre 2015 a
          2021
          segundo a Anvisa.</h3>
        <br>
      </v-container>

      <v-container class="bg-green-darken-4 mt-12 pt-5 elevation-24 border rounded-xl">

        <h2 class="font1 d-flex align-center justify-center border rounded-xl bg-black"><span
            :class="smAndDown ? 'pl-5' : ''">AUMENTO NO NÚMERO DE IMPORTAÇÕES
          </span></h2>
        <br>
        <h3 class="text-black">
          Dados da Anvisa informam um aumento de mais de 2.400% em seis anos no número de pedidos de importação de
          cannabis
          medicinal, média de 400% ao ano. Para se ter uma ideia melhor, em 2015 foram apenas 896 pedidos enquanto em 2021
          já se passava de 22 mil até o mês de setembro.
          O crescimento elevado na quantidade de solicitações de importação de produtos à base de cannabis fez com que a
          Anvisa avançasse em sua legislação aprovando a RDC 570/2021 visando diminuir o tempo de aprovação do cadastro,
          possibilitando o acesso mais rápido ao tratamento e com menos burocracia.
        </h3>
      </v-container>

      <br>

      <v-container class="mt-7 pt-5 elevation-24 border rounded-xl"
        :style="{ 'background-image': 'url(\'fundo2.jpg\')', 'background-size': 'cover' }">


        <h2 class="font1 d-flex align-center justify-center text-white bg-black border rounded-xl"><span
            :class="smAndDown ? 'pl-5' : ''">VOCÊ SABIA QUE A MAIOR
            PARTE DA POPULAÇÃO BRASILEIRA É A FAVOR DO USO MEDICINAL ?</span></h2>

        <br>
        <div class="d-flex align-center justify-center">
          <h3 class="text-white">Segundo pesquisa realizada pelo polo de negócios de impacto cívico-sócio-ambiental
            CIVI-CO,
            intitulado “Cannabis é saúde”, <span class="text-lime-accent-3">70% da população brasileira apoia a medicina
              canabinoide</span>. O levantamento realizado
            em 2021 contou com a participação de mil pessoas de todas as regiões do país.</h3>

          <v-img src="../public/marcha.jpg" width="300" :class="smAndDown ? 'w-0' : ''"></v-img>
        </div>

        <br>

        <v-dialog width="500">
          <template v-slot:activator="{ props }">
            <v-btn color="#C6FF00" width="300" class="ml-16" v-bind="props" text="Países legalizados"
              :class="smAndDown ? 'ml-auto' : ''"> </v-btn>
          </template>

          <template v-slot:default="{ isActive }">
            <v-card title="Paises legalizados">
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

        <br>
        <br>
        <br>

        <div class="d-flex align-center justify-center">
          <h1 class="font1 text-white">Não compre <svg-icon color="#C6FF00" type="mdi" :path="path"></svg-icon> plante!
          </h1>
        </div>
      </v-container>

      <v-container class="bg-green-darken-4 mt-12 pt-5 elevation-24 border rounded-xl"
        :style="{ 'background-image': 'url(\'../public/.jpg\')', 'background-size': 'cover' }">

        <h2 class="font1 d-flex align-center justify-center border rounded-xl bg-black">EVOLUÇÃO SOCIAL</h2>
        <br>
        <h3 class="text-black">
          A cannabis medicinal experimentou uma notável evolução social e legal nas últimas décadas. Inicialmente
          estigmatizada e proibida em muitos países, <span class="text-lime-accent-3">a planta agora é amplamente
            reconhecida por seus benefícios
            terapêuticos</span>.
          Várias nações, incluindo o Canadá, alguns estados dos Estados Unidos, e muitos outros países, legalizaram tanto
          o
          uso medicinal quanto o recreativo da cannabis. Essa mudança de mentalidade foi impulsionada por uma crescente
          base
          de evidências científicas que apoiam a eficácia da cannabis no tratamento de condições como dor crônica,
          epilepsia, ansiedade, entre outras.
          A pesquisa médica continua a explorar os inúmeros compostos da planta, incluindo o canabidiol (CBD) e o
          tetrahidrocanabinol (THC), e seus usos potenciais em uma variedade de tratamentos. Isso levou ao desenvolvimento
          de produtos à base de cannabis com concentrações controladas desses compostos para atender às necessidades
          específicas dos pacientes.
          A regulamentação da cannabis medicinal varia consideravelmente de um lugar para outro, mas geralmente visa
          garantir a segurança e a qualidade dos produtos. Além disso, a aceitação social da cannabis medicinal está
          crescendo, reduzindo o estigma associado a seu uso.
          À medida que a pesquisa continua a avançar e mais países consideram a legalização da cannabis, é provável que a
          evolução dessa planta no meio social continue, proporcionando mais acesso a tratamentos baseados em cannabis
          para
          pacientes em todo o mundo.
        </h3>
        <br>

        <h2 class="font1 d-flex align-center justify-center border rounded-xl bg-black" :class="smAndDown ? 'pl-5' : ''">
          IMPORTÂNCIA NA SOCIEDADE</h2>
        <br>
        <h2 class="font1">TRATAMENTO ALTERNATIVO :</h2>
        <h3 class="text-black">A cannabis medicinal oferece uma alternativa para pacientes que não encontraram alívio com
          tratamentos convencionais. Isso é especialmente relevante para aqueles que sofrem de condições crônicas, como a
          dor persistente, que podem não responder bem a tratamentos tradicionais.</h3>

        <br>

        <h2 class="font1">CONTROLE DE SINTOMAS :</h2>
        <h3 class="text-black">A cannabis tem mostrado eficácia no controle de sintomas em várias condições, como a
          redução
          de náuseas e vômitos em pacientes submetidos à quimioterapia, a melhoria do sono em pessoas com insônia e o
          alívio
          de espasmos musculares em pacientes com esclerose múltipla.</h3>

        <br>

        <h2 class="font1">REDUÇÃO DO USO DE OPIOIDES :</h2>
        <h3 class="text-black">O uso excessivo de opioides é uma preocupação de saúde pública. A cannabis medicinal pode
          servir como uma alternativa mais segura para o tratamento da dor, potencialmente reduzindo o risco de
          dependência.
        </h3>
        <br>

        <h2 class="font1">PESQUISA E INOVAÇÃO :</h2>
        <h3 class="text-black">O crescente interesse na cannabis medicinal está impulsionando a pesquisa e a inovação.
          Isso
          pode levar ao desenvolvimento de novos tratamentos e medicamentos baseados em compostos encontrados na cannabis.
        </h3>

        <br>

        <h2 class="font1">RECONHECIMENTO LEGAL :</h2>
        <h3 class="text-black"> À medida que mais países legalizam a cannabis medicinal, os pacientes têm um acesso mais
          fácil a tratamentos que antes eram proibidos. Isso também pode abrir portas para pesquisas clínicas mais amplas.
        </h3>

        <br>

        <h2 class="font1">POTENCIAL ECONÔMICO :</h2>
        <h3 class="text-black">A indústria da cannabis medicinal está crescendo e criando oportunidades econômicas
          significativas. A legalização da cannabis tem o potencial de gerar empregos e receita fiscal em muitas regiões.
        </h3>

        <br>

        <h2 class="font1">MUDANÇA NAS ATITUDES SOCIAIS :</h2>
        <h3 class="text-black">À medida que a cannabis medicinal ganha aceitação, as atitudes sociais estão mudando. O
          estigma associado ao uso da cannabis está diminuindo, o que permite que mais pacientes busquem tratamentos
          baseados na planta sem medo de preconceito.
        </h3>

        <br>

        <h2 class="font1">CUSTOMIZAÇÃO DE TRATAMENTOS :</h2>
        <h3 class="text-black">A variedade de cepas de cannabis e métodos de consumo permite que os tratamentos sejam
          adaptados às necessidades individuais dos pacientes. Isso pode levar a uma abordagem mais personalizada para o
          atendimento médico.
        </h3>

        <br>

        <h2 class="font1">REDUÇÃO DE CUSTOS DE SAÚDE :</h2>
        <h3 class="text-black">Se a cannabis medicinal for usada eficazmente para tratar condições de saúde, isso pode
          potencialmente reduzir os custos de saúde a longo prazo, uma vez que algumas terapias baseadas em cannabis podem
          ser mais acessíveis do que opções convencionais.
        </h3>

        <br>

        <h2 class="font1" :class="smAndDown ? 'ml-2' : ''">ACEITAÇÃO INTERNACIONAL :</h2>
        <h3 class="text-black">A legalização da cannabis medicinal em um número crescente de países está promovendo a
          aceitação internacional da planta como uma ferramenta terapêutica válida.
          A cannabis medicinal está desempenhando um papel cada vez mais importante no cenário médico e social, oferecendo
          esperança e alívio para muitos pacientes, ao mesmo tempo em que impulsiona a pesquisa e a inovação na área da
          saúde.
        </h3>
      </v-container>

      <v-container class="bg-green-darken-4 mt-16 pt-5 elevation-24 border rounded-xl">

        <h3 class="text-center text-black">"Hoje em dia está absolutamente demonstrado, não há razão, a não ser
          ideológica, para rejeitar a verdade de
          que a maconha tem efeitos terapêuticos plenamente comprovados."</h3>
        <br>
        <h1 class="font1 text-center">Dr. Elisaldo Carlini</h1>

      </v-container>

      <v-container class="bg-white mt-16 pt-5 elevation-24 border rounded-xl d-flex justify-center align-center">
        <h3 class="text-center text-black">“A importância de falar sobre a Cannabis é total, porque é muito satisfatório
          para mim quanto profissional e para o paciente colher os benefícios e ter seus objetivos atingidos
          terapeuticamente com esse fitofármaco. Além disso, é importante até uma questão de renivelação civilizatória que
          o Brasil tem que passar para acompanhar países que estão mais desenvolvidos no assunto. Então é importante
          discutir, conversar e levar conhecimento. Pois a ignorância é o que gera o sofrimento”
          <p></p>
          <h1 class="mt-10">Dr. Vinicius Mesquita</h1>
        </h3>

        <v-img src="../src/assets/images/logomed.jpg" width="300" height="300" :class="smAndDown ? 'w-0 h-0' : ''"></v-img>

      </v-container>

      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>

      <v-footer class="bg-black align-center justify-center mt-10">
        <v-chip color="white" href="https://github.com/luanmello777" target="_blank>"><svg-icon type="mdi" :path="path1"
            class="mr-2"></svg-icon>github.com/Luanmello777
        </v-chip>
      </v-footer>


    </v-main>
  </v-img>
</template>


<style scoped>
.small-text {
  font-size: 12.5px;
}

.bg-white {
  font-size: 13px;

}
</style>


<script setup>
import { useDisplay } from 'vuetify';
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiCannabis, mdiGithub } from '@mdi/js';

const { smAndDown } = useDisplay()

const path = mdiCannabis;
const path1 = mdiGithub;
const items = ['Estados Unidos', 'Israel', 'Colômbia', 'Holanda', 'México', 'Uruguai', 'Espanha', 'Alemanha']

</script>

