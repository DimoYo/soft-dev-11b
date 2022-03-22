<script>
    export let leave = 0;
    let onleave = () =>{
        leave = 0;
    }
    let players = "3";
</script>
<style>
:global(body){
        background-image: url('./background.png');
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-size: 100% 100%;
	}
    .box{
        font-family: 'Nova Round';
        
        position: absolute;
        width: 800px;
        height: 190px;
        top: 200px;

        background: radial-gradient(50% 50% at 50% 50%, #5F7DC9 0%, rgba(85, 222, 115, 0) 100%);
    }
    h1{
        font-family: Nova Round;
        background: -webkit-linear-gradient(rgba(0, 255, 41, 1), rgba(0, 240, 255, 1));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        
        font-style: normal;
        font-weight: normal;
        font-size: 50px;
        line-height: 120px;
        text-align: center;
    }
    h3{
        position: absolute;
        width: 800px;
        height: 62px;
        top: 214px;
        
        display: flex;
        justify-content: center;
            
        font-family: Nova Round;
        background: -webkit-linear-gradient(rgba(0, 255, 41, 1), rgba(0, 240, 255, 1));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        
        font-style: normal;
        font-weight: normal;
        font-size: 40px;
        line-height: 42px;
        text-align: center;
    }
    .centerred{
		position: absolute;
		left: 30%;
		top: 10%;
		transform: translate(-50%, -50%);
	}
</style>
<div class = "centerred">
<div class="box">
    <h1>Searching for a game...<br/><a href = "/Mainpage/">click to leave</a></h1>
    <h3 >Found {{players}}/4 players...</h3>
</div>
</div>