<template>
  <div class="container">
    <Header/>
    <div class="frame">
      <Menu/>
      <div class="content_column">
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <Column>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
          <Card/>
        </Column>
        <button class="add_column">+ New Column</button>
      </div>
    </div>
  </div>
  
</template>

<script>
import Header from "./components/Header.vue";
import Menu from "./components/Menu.vue";
import Card from "./components/Card.vue";
import Column from "./components/Column.vue";

export default {
  name: 'App',
  components: {
    Header,
    Menu,
    Card,
    Column
  }
 
}
</script>

<style>
.container{
  display: flex;
  flex-direction: column;
  background-color: var(--light-grey);
}

.frame{
  display: flex;
  width: 100%;
  height: 100%;
}

.content_column{
  display: flex;
  width: 100%;
  height: calc(100vh - 95px);
  overflow: auto;
}

.add_column{
  min-width: 250px;
  min-height: 100vh;
  margin: 75px 24px 24px 24px;
  border-radius: 6px;
  background-color: var(--lines-light);
  font-weight: 700;
  font-size: 24px;
  line-height: 30px;
  text-align: center;
  color: var(--medium-grey);
}
.add_column:hover{
  color: var(--main-color);
  background-color: var(--lines-light);
}

</style>
