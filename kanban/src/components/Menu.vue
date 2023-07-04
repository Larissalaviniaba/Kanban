<template>
    <div class="container_menu" v-show="showElement">
        <div class="content_menu" v-if="showElement">
            <h3 class="boards_title">ALL BOARDS (3)</h3>
            <div class="list_boards">
                <button class="board_add"> <i class="ph ph-kanban"></i> + Create  New Board</button>
                <button class="board board_selected" ><i class="ph ph-kanban"></i> Platform Launch</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Roadmap</button>
                <button class="board"><i class="ph ph-kanban"></i> Platform Launch</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Roadmap</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Roadmap</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Roadmap</button>
                <button class="board"><i class="ph ph-kanban"></i> Marketing Plan</button>
                <button class="board"><i class="ph ph-kanban"></i> Roadmap</button>
            </div>
        </div>
        
        <div class="group_down">
            <div class="btn_theme">
                <i class="ph ph-sun"></i>
                <input type="checkbox" v-model="isChecked" @change="checkboxChanged" id="darkmode-toggle"/>
                <label for="darkmode-toggle"></label>
                <i class="ph ph-moon"></i>
            </div>
            <button @click="this.showElement = false" class="hide"> <i class="ph ph-eye-slash"></i>Hide Sidebar</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Menu',
    data() {
        return {
            showElement: true
        };
    },
    methods:{
        
    },


}
</script>

<style scoped>
.container_menu{
    display: flex;
    flex-direction: column;
    width: 295.5px;
    max-height: calc(100vh - 95px); 
    padding-right: 5px;
    background-color: var(--white);
}

.ph{
    margin-right: 16px;
}

.content_menu{
    max-height: calc(100% - 123px);
}

.list_boards{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    width: 100%;
    height: 100%;
    overflow-x: auto;
}

.boards_title{

    width: 100%;
    height: 15px;

    font-weight: 700;
    font-size: 12px;
    line-height: 15px;
    letter-spacing: 2.4px;
    padding: 32px 32px;

    color: var(--medium-grey);
}

.board{
    min-height: 48px;
    font-weight: 700;
    font-size: 15px;
    line-height: 19px;
    padding-left: 32px;
    color:var(--medium-grey);
    border-radius: 0px 100px 100px 0px;
    transition: 0.2s;
}

.board:hover{
    color:var(--main-color);
    background-color: var(--lines-light)
}

.board_selected{
    background: var(--main-color);
    border-radius: 0px 100px 100px 0px;
    color: var(--white);
}
.board_add{
    min-height: 48px;
    font-weight: 700;
    font-size: 15px;
    line-height: 19px;
    padding-left: 32px;
    border-radius: 0px 100px 100px 0px;
    color:var(--main-color);
    transition: 0.2s;
}
.board_add:hover{
    color:var(--main-color);
    background-color: var(--lines-light)
}
.group_down{
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 123px;
    background-color: var(--white);
    padding: 20px 0px;
}
.btn_theme{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 200px;
    height: 48px;
    background: var(--light-grey);
    border-radius: 6px;
    margin-left: 15px;
    margin-right: 15px;
}

.btn_theme > label {
    width:45px;
    height:20px;
    position: relative;
    display: block;
    background-color: var(--medium-grey);
    border-radius: 200px;
    box-shadow: inset 0px 5px 15px rgba(0,0,0,0.), inset 0px -5px 15px rgba(255,255,255,0.4);
    cursor: pointer;
    margin-right: 10px;
}
.btn_theme > label:after {
    content: "";
    width:14px;
    height: 14px;
    position: absolute;
    top:3px;
    left:4px;
    background-color: var(--white);
    border-radius: 14px;
    box-shadow: 0px 5px 10px rgba(0,0,0,0.2);
}
.btn_theme > input {
    width: 0;
    height: 0;
    visibility: hidden;
}
.btn_theme > input:checked + label {
    background: var(--main-color);
}
.btn_theme > input:checked + label:after {
    left:29px;
    transform: translateX(-10%);
    background: var(--white);
}
.btn_theme > label, label:after {
    transition: 0.3s
}
.btn_theme > label:active:after{ 
    width: 14px; 
}
.btn_theme > .ph{
    color: var(--medium-grey)
}
.hide{
    max-width: 100%;
    min-height: 48px;
    font-weight: 700;
    font-size: 15px;
    line-height: 19px;
    padding-left: 32px;
    margin-top:5px ;
    color:var(--medium-grey);
    border-radius: 0px 100px 100px 0px;
    transition: 0.2s;
}
.hide:hover{
    color:var(--main-color);
    background-color: var(--lines-light)
}
</style>