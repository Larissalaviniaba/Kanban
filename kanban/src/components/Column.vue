<template>
    <div class="column">
        <div class="title">
            <p class="color"></p>
            <h3>TODO (4)</h3>
        </div>
        <slot class="content"></slot>
    </div>
</template>

<script>
export default {
    name: 'Column',

}
</script>

<style scoped>
.column{
    width: 280px;
    min-height: 100vh;
    padding: 24px calc(24px - 12px) 24px 24px;
    margin-top: 15px;
}
.title{
    display: flex;
    justify-content: flex-start;
    align-items: center;

    font-weight: 700;
    font-size: 12px;
    line-height: 15px;
    letter-spacing: 2.4px;
    color: var(--medium-grey);
}

.color{
    width: 15px;
    height: 15px;
    border-radius: 50%;
    margin-right: 10px;
    background-color: blueviolet;
}

.content{

}

</style>