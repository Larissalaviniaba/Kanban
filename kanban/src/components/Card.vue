<template>
    <div class="card">
        <h3>Build UI for search</h3>
        <p>0 of 1 substasks</p>
    </div>
</template>

<script>
export default {
    name: 'Card',

}
</script>

<style scoped>
.card{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-width: 250px;
    min-height: 88px;
    background-color: var(--white);
    box-shadow: 0px 4px 6px rgba(54, 78, 126, 0.101545);
    border-radius: 8px;
    margin-bottom: 10px;
    margin-top: 20px;
    
    padding: 12px 15px;
    transition: box-shadow 0.3s ease;
    cursor: pointer;
    color: var(--black);
    

}
.card:hover{
    color: var(--main-color);
    box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
}
h3{
    width: 80%;
    padding-bottom:10px ;
    font-weight: 700;
    font-size: 15px;
    line-height: 19px;
}
p{
    width: 80%;
    font-weight: 700;
    font-size: 12px;
    line-height: 15px;
    color: var(--medium-grey);
}

</style>