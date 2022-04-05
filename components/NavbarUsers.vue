<template>
    <div>
    <div class="header">
        <input placeholder="Поиск по теме"/>
        <div class="user">
            <img src="https://t4.ftcdn.net/jpg/00/64/67/63/360_F_64676383_LdbmhiNM6Ypzb3FM4PPuFP9rHe7ri8Ju.jpg" alt="avatar"/>
        <div class="info">
            <h4>name</h4>
            <p>the role</p>
        </div>
        </div>
    </div>

  
    </div>
</template>

<script>
    export default {
        name: 'NavbarUsers'
    }
</script>

<style scoped>
input{
    padding: 10px 10px 10px 10px;
    font-size: 17px;
    border-radius: 10px;
    border-color: rgba(170, 170, 170, 0.753);
    width: 100%;
    max-width: 400px;
    height: 20px;
}
.header{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
}
.user{
    display: flex;
    align-items: center;
    
}

</style>