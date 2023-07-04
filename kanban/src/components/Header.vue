<template>
    <header>
        <div class="group_logo">
            <img class="logo" src="../assets/logo (3).png" alt="Logo">
            <h1 class="title">Kanban</h1>
        </div>
        <div class="header">
            <p>Platform Launch</p>
            <button class="button_primary_l">+ Add New Task</button>
            <button class="button_options"><i class=" ph ph-dots-three-vertical"></i></button>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',

}
</script>

<style scoped>

header{
    display: flex;
    background-color: var(--white);
    width: 100%;
}
.header{
    display: flex;
    justify-content: center;
    align-items: center;
    width: calc(100% - 250px);
    height: 95px;
    padding: 0px 10px 0px 32px;
    background-color: var(--white);
    box-shadow: 0 2px 4px rgba(65, 64, 64, 0.2);
}
.group_logo{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 250px;
    box-shadow: 0 2px 4px rgba(65, 64, 64, 0.2);
  }
  
  .logo{
    width: 24px;
    height: 25px;
  }
  .title{
    width: 150px;
    height: 30px;
    font-weight: 800;
    font-size: 24px;
    line-height: 30px;
    color: var(--black);
    margin-left: 16px;
  }

p{
    width: 80%;
    font-weight: 700;
    font-size: 24px;
    line-height: 30px;
    color: var(--black);
}
.button_options{
    width: 50px;
    height: 50px;
    margin-left: 24px;
}

.ph{
    color: var(--medium-grey) !important;
    font-size: 30px ;
}

</style>