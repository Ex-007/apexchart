<template>
    <div class="container">
        <aside class="routerr">
            <div class="side">
                <h4 class="aOptions">Option 1</h4>
                <h4 class="aOptions">Option 2</h4>
                <h4 class="aOptions">Option 3</h4>
                <h4 class="aOptions">Option 4</h4>
                <h4 class="aOptions">Option 5</h4>
            </div>
        </aside>
        <main class="main">
                <div class="top">
                    <div class="topOne">
                        
                    </div>
                    <div class="topTwo">

                    </div>
                </div>
                <div class="bottom">
                    <div class="bottomOne">

                    </div>
                    <div class="bottomTwo">

                    </div>
                    <div class="bottomThree">

                    </div>
                </div>
        </main>
    </div>
</template>

<style scoped>
    .container{
        display: grid;
        grid-template-columns: 20% 80%;
        height: 100vh;
    }
    .routerr{
        color: white;
        padding: 5px;
        background-color: rgb(66, 48, 48);
        overflow-y: auto;
        display: grid;
        grid-template-columns: 1fr;
        text-align: center;
    }
    .main{
        padding: 5px;
        display: grid;
        grid-template-columns: 1fr;
    }
    .aOptions{
        background-color: white;
        height: 30px;
        border-radius: 20px;
        color: rgb(66, 48, 48);
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
    }
    .aOptions:hover{
        background-color: rgb(66, 48, 48);
        color: white;
        border: 2px solid white;
    }
    .top{
        background-color: rgb(184, 143, 89);
        display: grid;
        grid-template-columns: 2fr 1fr;
    }
    .topOne{
        background-color: black;
    }

    .bottom{
        background-color: rgb(91, 154, 154);
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
    }
    .bottomOne{
        background-color: white;
    }
    .bottomThree{
        background-color: rgb(180, 46, 46);
    }
</style>