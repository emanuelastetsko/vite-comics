<script>


export default {
    name: 'AppHeader',
}

</script>


<template>

    <header>

        <div class="my-container">
            <div class="header-flex">
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="Logo">
                </div>
                <div class="navbar">
                    <ul>
                        <li>CHARACTERS</li>
                        <li>COMICS</li>
                        <li>MOVIES</li>
                        <li>TV</li>
                        <li>GAMES</li>
                        <li>COLLECTIBLES</li>
                        <li>VIDEOS</li>
                        <li>FANS</li>
                        <li>NEWS</li>
                        <li>SHOP</li>
                    </ul>
                </div>
            </div>
            
        </div>

    </header>

</template>


<style lang="scss" scoped>

.header-flex{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 0;
}
.logo img{
    width: 60px;
    height: 60px;
}

ul{
    display: flex;
    list-style: none;
    
    li{
        padding: 0 7px;
    }
}

</style>