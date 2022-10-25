<template>
    <div>
        <table :id="sId" @mouseover="doHighlight" @mouseleave="ceaseHighlight" :class="{main: hovering, oferta: this.oferta != null && hovering}">
            <tr>
                <td class="subject" rowspan="3">{{subject}}</td>
                <td class="carga" rowspan="2">{{carga}}</td>
            </tr>
            <tr>       
            </tr>
            <tr>
                <td class="cr">{{cr}}</td>
            </tr>    
        </table>
    </div>
</template>

<script>
export default {
    name: 'Subject',
    props: ['subject', 'carga', 'cr', 'sId', 'pre', 'oferta'],
    methods: {
      doHighlight() {
        this.hovering = true;
        const preRequisites = this.pre.split(',');
        preRequisites.map( (subject) => document.getElementById(subject).classList.add('pre'));
        
        // this.pre.
      },
      ceaseHighlight() {
        this.hovering = false;
        const preRequisites = this.pre.split(',');
        preRequisites.map( (subject) => document.getElementById(subject).classList.remove('pre'));
      }
    },
    data() {
      return {
        hovering: false
      }
    }
}
</script>

<style scoped>
table {
    border: 1px solid #000;
    border-collapse: collapse;
    margin: 20px 2px;
    cursor: pointer;    
}

tr, td {
  border: 1px solid #000;    
}

.subject {
  padding: 0px 30px;
  width: 160px;
  height: 60px;
  max-width: 160px;  
  max-height: 60px;
  text-align: center;
  box-sizing: border-box;    
}

.cr {
  padding: 2px 10px;
}

.carga {
  padding: 20px 10px 2px 10px;  
}

body {
  font-family: arial;
}

.main {
  background-color: #A2D3C2;
}

.pre {
  background-color: #EAD637;
}

.oferta {
  background-color: #D6F49D;
}

</style>