<template>
	<div>
		<nav id="rootNav"  class="navbar navbar-expand-sm navbar-light bg-academy fixed-top" data-toggle="affix">
		  <div class="container">
		        <a href="/" class="navbar-brand lato navbar-realacademy">🥇 Kubo Store </a>
		        <button class="navbar-toggler float-right" type="button" data-toggle="collapse" data-target="#navbar-test">
		            <span class="navbar-toggler-icon"></span>
		        </button>
		        
	        	<div class="navbar-collapse collapse" id="navbar-test">
					<ul class="navbar-nav ml-auto">	
						<li class="nav-item">
				            <a class="nav-link" href="/">Inicio</a>
				        </li>

				        <li class="nav-item">
				            <a class="nav-link" href="/orders">Pedidos</a>
				        </li>
				        <li class="nav-item">
				            <a class="nav-link" href="/about">Acerca de</a>
				        </li>

					</ul>
					<ul class="navbar-nav ml-auto">	
						
				        <li class="nav-item">
				            <a class="nav-link" href="javascript:void(0);">
				            	<img src="https://image.flaticon.com/icons/svg/1177/1177568.svg" style="width:25px" alt="">Mi cuenta
				            </a>
				        </li>				        
				        <li class="nav-item" v-on:click="llamado()">
				            <a class="nav-link" href="javascript:void(0);">
				            	<img src="https://image.flaticon.com/icons/svg/891/891581.svg" style="width:25px" alt="">Carrito  <span id="quantity" class="bold"></span>
				            </a>
				        </li>
					</ul>					
	      		</div>
	    </div>
	   </nav>
	 </div>
</template>	

<script>
	export default{	
	
		data(){
			return {
				user : []
			}
		},
		props : {
			callTo: "",
		},		
		methods: {
			llamado(){
				this.callTo('openCartList');
			}
		},

		mounted(){
			
			

		}

	}
</script>