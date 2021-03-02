<template>
  <header class="Entete">
    <div id="initiale">
      mld
    </div>
    <ul class="nav">
      <li>portfolio</li>
      <li>à propos</li>
      <li>contact</li>
      <li id="lang">
        <span>en</span> 
        <span>|</span>
        <span>fr</span>
      </li>
    </ul>

  </header>
</template>

<script>
export default {
  name: 'Entete'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Entete{
  background-color: #FFA4B0;
  position: sticky;
  top: 0;
  z-index: 10;
  height: 5vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: white;
  font-size: 1.5em;
  padding: 5vh 3vh;
}

#initiale{
  font-family:'Pacifico', cursive;
  font-size: 1.5em;
}

ul{
  display: flex;
  /* margin: 10px 0 0 0; */
  padding: 0;
  list-style: none;
  font-size: 0.8em;
  align-items: center;
}

li{
  cursor: pointer;
  padding-left: 30px;
}
li:first-child{
  padding: 0;
}

#lang{
  display: flex;
  flex-flow: row;
  align-items: center;
}

#lang div{
  padding-right: 2.5px;
}

#lang div:last-child{
  padding-left: 0;
  padding-left: 2.5px;
  color: #FC6478;
}
</style>
