<template>
  <div id="App">
    <div class ="listbox">
    <br>
    <ejs-combobox :dataSource='dataItem' :fields='dataFields'
    placeholder='Zvol web' popupWidth="250px" 
    popupHeight="200px" sortOrder="Descending" allowFiltering ='true' >
    </ejs-combobox>
    </div>
     <div class="Nazev_loga">
<span>Checked names: {{}} </span>

  </div> <div class="logo">
   <img src="https://www.w3schools.com/images/w3schools_green.jpg" width="250" height="250">
    </div>

  </div>

</template>

<script>


import Vue from "vue";
import { ComboBoxPlugin} from '@syncfusion/ej2-vue-dropdowns';
Vue.use(ComboBoxPlugin);

export default Vue.extend({
  data: function() {
    return {

      
      dataItem: [
        {Name:'Idnes.cz', ID:'item1'},
          {Name:'Novinky.cz', ID:'item1'},
            {Name:'tncz.cz', ID:'item1'},
              {Name:'mladafrontadnes.cz', ID:'item1'},
                {Name:'nava.cz', ID:'item1'},
                  {Name:'asdf.cz', ID:'item1'}

      ],
      dataFields: {value: 'ID', text: 'Name'}
    };
  }
});

</script>


<style>


.listbox{
padding-top: 20%;
width: 250px;

}
.Nazev_loga{
padding-top: 10;
text-align: center;
}
.logo img
{
padding: 40%;
}
@import url(https://cdn.syncfusion.com/ej2/material.css);
</style>