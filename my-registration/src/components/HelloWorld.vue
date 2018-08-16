<template>
  <div class="hello">
    <div v-bind:class="{active:isactive}"><h3><center>{{ msg }}</center></h3></div>
    <div class="position">
      <center>
    <table>
      <tr>
        <td><label1><label>FULL NAME:</label></label1>
        <input v-model="fullname" placeholder="" type="text"></td>
      </tr>
      <tr>
        <td><label1><label>EMAIL_ID:  </label></label1>
        <input v-model="email" placeholder="" type="text"></td>
        </tr>
      <tr>
        <td><label1><label>MOBILE:</label></label1>
        <input v-model="mobile" placeholder="MOBILE" type="text"></td>
      </tr>
    <tr>
        <td><label1><label>Country:</label></label1>
        <select v-model="country">
          <option>Canada</option>
          <option>USA</option>
          <option>India</option>
          <option>Japan</option>
          <option>Singapore</option>
        </select></td>
    </tr>
    <center>
      <h4>Cloud Regions Offered</h4>
        <input type="radio" value="eastus" v:model="radiopicks">
        <label>EastUS</label>
        <input type="radio" value="southasia" v:model="radiopicks">
        <label>SouthAsia</label>
    </center>
        <br/><br/>

</table>
      </center>
        <h4>SERVICES OFFERED</h4>
        <center>
        <table>
          <tbody>
            <tr>
              <td><input type="checkbox" value="Virtual">
              <label>VM Services</label></td>
             <td> <input type="checkbox" value="Container">
              <label>Container Services</label></td>
              <td><input type="checkbox" value="storage">
                  <label>Storage Services</label></td>
              </tr>
        <tr>
        <td><input type="checkbox" value="Domain">
        <label>Domain Services</label></td>
        <td><input type="checkbox" value="software">
        <label>Licensed Software Services</label></td>
        <td><input type="checkbox" value="Hybrid">
        <label>Hybrid Cloud Services</label></td>
        </tr>
        </tbody>
        </table>
        <br/>
        <input type="button" value="SIGN UP!">
        </center>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'SIGN UP ON TO OUR CLOUD',
      isactive: true
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.active{
  color:blue;
  font-size: 20px;
}
.position{
  align-content: center;
  margin-bottom: 15px;
}
label1 {
    width:100px;
    clear:left;
    text-align:right;
    padding-right:10px;
}

input1, label1 {
    float:left;
}
</style>
