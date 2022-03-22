<style>

        :global(body){
            background-image: url('./image 1.png');
        }
		.parent{
			flex-wrap: wrap;
			padding: 0 4px;
			
			height: 850px;
			display: flex;
			align-items: center;
			justify-content: center;

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
			
			margin-top: 1px;
			margin-right: 2px;
			position: absolute;
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
</style>
<button class="button"><i class="fa fa-bars"></i></button>
	
<div class="parent">
    <img alt = "Duska" src="Assets/board.jpg">
</div>
