<script>
    export let window = 0;
    let change_to_find_team_belot = ()=>{
        window = 1;
    }
    let change_to_find_team_uno = ()=>{
        window = 1;
    }
    let dropdown_login = 0;
    let dropdown_login_toogle = ()=>{
        if(dropdown_login == 0){
            dropdown_login = 1;
        }else{
            dropdown_login = 0;
        }
    };
</script>  
<style>
    @import url('https://fonts.googleapis.com/css2?family=Nova+Round&family=Zen+Dots&display=swap');
    :global(body){
        background-image: url('./background.png');
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-size: 100% 100%;
	}

h1{
    font-size: 1000%;
    color: rgb(170, 170, 170);
    text-align: center;
    font-family: 'Zen Dots';
}

.button{
    background-color: #a5a5a59a;
    border: none;
    color: white;
    padding: 10px 22px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 250%;
    font-family: 'Nova Round';
    border-radius: 40px;
    box-shadow: 0px 0px 2px 2px black;
    cursor: pointer;
    margin: 5px;
}

.long{
    width: 330px;
    margin: 0 auto;
}

.uno{width: 125px;}
.belot{width: 195px;}

.topRight{
    margin-top: 1px;
    margin-right: 2px;
    position:absolute;
    top: 10px;
    right: 10px;
}

.button:hover{
    background-color:#ffffff9a;
    transition: 0.2s;
    color: #e7e7e7;
}

.button:active{
    background-color:white;
}

.column{
    display: flex;
    flex-direction: column;
    flex: 1;
    overflow: visible;
    align-items: center;
    justify-content: center;
    margin-bottom: 50px;
}

.row{
    display: flex;
    flex-direction: row;
    flex: 1;
    overflow: visible;
    align-items: center;
    justify-content: center;
}


.Hdivider{
    height: 5px;
    display: inline-block;
}

.menu{
    margin-top: 1px;
    margin-right: 2px;
    position:absolute;
    top: 45px;
    right: 50px;
    box-shadow: 0px 0px 2px 2px black;
    height: 425px;
    width: 300px;
    background-color: #433f3f7c;
}

.picture{
    margin-top: 1px;
    margin-right: 2px;
    position:absolute;
    top: 70px;
    right: 105px;
}

.login{
    width: 200px;
    margin-top: 1px;
    margin-right: 2px;
    position:absolute;
    top: 300px;
    right: 100px;
}

.signup{
    width: 200px;
    margin-top: 1px;
    margin-right: 2px;
    position:absolute;
    top: 375px;
    right: 100px;
}
</style>

<div>
<h1>TITLE</h1>

<div>
    <button class="button topRight" on:click={dropdown_login_toogle}><i class="fa fa-bars"></i></button>
</div>

{#if  dropdown_login == 0}
<div class="menu"></div>
<img src="/Assets/profile.png" alt="Profile Picture" class="picture"/>
    <div>
        <button class="button login">Log in</button>
        <button class="button signup">Sign up</button>
    </div>
{/if}


<div class="row">
    <a href="/SearchGame/"><button class="button uno" on:click = {change_to_find_team_uno}> UNO</button></a>
    <a href="/SearchGame/"><button class="button belot" on:click = {change_to_find_team_belot}>BELOT</button></a>
</div>

<div class="column">
    <button class="button long">CREATE ROOM</button>
    <div class="Hdivider"></div>
    <button class="button long">FIND ROOM</button>
    <div class="Hdivider"></div>
    <button class="button long">SETTINGS</button>
</div>
</div>