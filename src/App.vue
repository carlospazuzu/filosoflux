<template>
  <div class="container">
    <div class="row">
      <h3>FLUXOGRAMA INTELIGENTE DO CURSO DE LICENCIATURA EM FILOSOFIA - UFPI</h3>      
    </div>
    <div class="row">
      <div class="col-2"></div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO I" />
        <Subject subject="Seminário de Introd. ao Curso de Fil." carga="15" cr="01" sId="seminario" />
        <Subject subject="Iniciação à Fil. e à Red. Filosófica" carga="75" cr="05" sId="iniciacao" ref="iniciacao" />
        <Subject subject="Introdução à Met. Científica (IMC)" carga="60" cr="04" sId="imc" />
        <Subject subject="Sociologia da Educação" carga="60" cr="04" sId="sociologiaeduc" />
        <Subject subject="Inglês Instr. I" carga="60" cr="04" sId="inglesfrances" />
        <Subject subject="História da Educação" carga="60" cr="04" sId="histeduc" />
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO II" />
        <Subject subject="História da Filosofia Antiga" carga="75" cr="05" sId="filosantiga" pre="iniciacao"/>
        <Subject subject="Lógica I" carga="60" cr="04" sId="logica1" pre="iniciacao"/>
        <Subject subject="Ontologia I" carga="60" cr="04" sId="ontologia1" pre="iniciacao"/>
        <Subject subject="Teoria do Conhec. I" carga="60" cr="04" sId="teoriaconhecimento1" pre="iniciacao"/>
        <Subject subject="Psicologia da Educação" carga="60" cr="04" sId="psicoeduc" />
        <Subject subject="Seminário em Fil. e Meio Ambiente" carga="15" cr="01" sId="semfilmeioamb" />
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO III" />
        <Subject subject="História da Filosofia Medieval" carga="75" cr="05" sId="filosmedieval" pre="filosantiga"/>
        <Subject subject="Tóp. Esp. em His. da Fil. Antiga" carga="30" cr="02" sId="topespfilantiga" pre="filosantiga"/>
        <Subject subject="Ontologia II" carga="60" cr="04" sId="ontologia2" pre="ontologia1"/>
        <Subject subject="Teoria do Conhec. II" carga="60" cr="04" sId="teoriaconhecimento2" pre="teoriaconhecimento1,logica1"/>
        <Subject subject="Introdução à Ética" carga="60" cr="04" sId="intetica" pre="ontologia1,filosantiga,logica1"/>
        <Subject subject="Legislação e Org. da Educ. Básica" carga="60" cr="04" sId="legisl"/>
        <Subject subject="Ativ. Complem." carga="60" cr=" " sId="ativcomp"/>
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO IV" />
        <Subject subject="História da Filosofia Moderna" carga="90" cr="06" sId="filosmoderna" pre="filosmedieval"/>
        <Subject subject="Teorias da Ética" carga="75" cr="05" sId="teoriasetica" pre="intetica,teoriaconhecimento2,filosmedieval,ontologia2"/>
        <Subject subject="Antropologia Filosófica I" carga="60" cr="04" sId="antfilos" pre="ontologia1,teoriaconhecimento1"/>
        <Subject subject="Avaliação de Aprendizagem" carga="60" cr="04" sId="avaliacao" oferta="true" />
        <Subject subject="Seminário em Filosofia (Optativa)" carga="30" cr="02" sId="seminariofilos" oferta="true" />
        <Subject subject="Didática Geral" carga="60" cr="04" sId="didatica" pre="imc" />
        <Subject subject="Ativ. Complem." carga="40" cr=" " sId="ativcomp"/>
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO V" />
        <Subject subject="História da Filosofia Contemp. I" carga="60" cr="04" sId="filoscontemp1" pre="filosmoderna"/>
        <Subject subject="Metodologia Filosófica" carga="75" cr="05" sId="metfilosofica" pre="filosmoderna,teoriaconhecimento2,logica1"/>
        <Subject subject="Tóp. Esp. em His. da Fil. Moderna" carga="30" cr="02" sId="topespfilmoderna" pre="filosmoderna"/>
        <Subject subject="Metodologia do Ens. de Filosofia" carga="60" cr="04" sId="metensfilos" pre="didatica,filosmoderna,ontologia2,teoriasetica"/>
        <Subject subject="Filosofia da Linguagem" carga="60" cr="04" sId="filoslinguagem" pre="teoriaconhecimento2,ontologia2"/>
        <Subject subject="Estágio Curricular Superv. I" carga="75" cr="05" sId="estagio1" pre="didatica"/>
        <Subject subject="Ativ. Complem." carga="40" cr=" " sId="ativcomp"/>
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO VI" />
        <Subject subject="História da Filosofia Contemp. II" carga="60" cr="04" sId="filoscontemp2" pre="filoscontemp1"/>
        <Subject subject="Filosofia da Educação" carga="60" cr="04" sId="filoseduc" pre="filosmoderna"/>
        <Subject subject="Seminário de Filosofia (Opt.)" carga="30" cr="02" sId="seminariofilos" oferta="true" />
        <Subject subject="Optativa" carga="60" cr="04" sId="optativa" oferta="true" />
        <Subject subject="Optativa" carga="60" cr="04" sId="optativa" oferta="true" />
        <Subject subject="Estágio Curricular Superv. II" carga="75" cr="05" sId="estagio2" pre="didatica,avaliacao,filoscontemp1,teoriaconhecimento2,ontologia2"/>
        <Subject subject="Ativ. Complem." carga="40" cr=" " sId="ativcomp"/>
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO VII" />
        <Subject subject="Filosofia no Brasil e na América Lat." carga="60" cr="04" sId="filosbrasil" pre="filoscontemp2"/>
        <Subject subject="Tópicos Especiais (Opt.)" carga="30" cr="02" sId="topespopt" oferta="true" />
        <Subject subject="Optativa" carga="60" cr="04" sId="optativa" oferta="true" />
        <Subject subject="Optativa" carga="60" cr="04" sId="optativa" oferta="true" />
        <Subject subject="Estágio Curricular Superv. III" carga="120" cr="08" sId="estagio3" pre="estagio2"/>
        <Subject subject="TCC I" carga="30" cr="02" sId="tcc1" pre="filoscontemp2,teoriasetica,filoslinguagem,ontologia2,teoriaconhecimento2,antfilos"/>
      </div>
      <div class="col-2">
        <ModuleHeader text="MÓDULO VIII" />
        <Subject subject="Optativa" carga="60" cr="04" sId="optativa" oferta="true" />
        <Subject subject="Optativa" carga="60" cr="04" sId="optativa" oferta="true" />
        <Subject subject="Tópicos Especiais (Opt.)" carga="30" cr="02" sId="topespopt" oferta="true" />
        <Subject subject="Estágio Curricular Superv. IV" carga="120" cr="08" sId="estagio4" pre="estagio3"/>
        <Subject subject="TCC II" carga="60" cr="04" sId="tcc2" pre="tcc1"/>
      </div>
      <div class="col-2"></div>      
    </div>    
  </div>
</template>

<script>
import Subject from './components/Subject.vue'
import ModuleHeader from './components/ModuleHeader.vue'

export default {
  name: 'App',
  components: {    
    Subject,
    ModuleHeader
  }
}
</script>

<style scoped>
.text-centered {
  text-align: center;
  margin: 0 auto;
}
</style>
