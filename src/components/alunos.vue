<template>
<div>
	<section class="barra">
		<h1 class="inicio" >Início</h1>
	</section>
	<ul class="alunos">
		<li class="aluno" v-for="aluno in alunos">
			{{aluno.name}},{{aluno.idade}}
		</li>
	</ul>
</div>
</template>
<script>
	export default {
		name:'alunos',
		data() {
			return {
				alunos:[
					{
						name:'Carla',
						idade:'33'
					},
					{
						name:'Nadine',
						idade:'24'
					},
					{
						name:'Patrik',
						idade:'29'
					},
					{
						name:'Jaime',
						idade:'21'
					},
											
				]
			}
		}
	}
</script>
<style>
*{  padding: 0;
	margin:0;
	box-sizing: border-box;
}
.alunos{
	margin: 0px;
	background-color: purple;
	height: 80vh;
	width: 100%;
	padding: 45px;
}
.aluno{
	display: inline-flex;
	margin: 20px;
	width: 80px;
	height: 80px;
	background-color: yellow;
	text-align: left;
}
.barra{
	display: block;
	margin: 0;
    padding-top: 13px;
    height: 82px;
    width: 100%;
    min-width: 980px;
	background-color: #3b5998;
    background-image: linear-gradient(#4e69a2, #3b5998 50%);
    border-bottom: 1px solid #133783;
    min-height: 42px;
    position: relative;
    z-index: 1;
}
.inicio{
	display: block;
	font-size: 29px;
	color: white;
    margin: 0;
    padding: 0;
    -webkit-margin-before: 0.67em;
    -webkit-margin-after: 0.67em;
    -webkit-margin-start: 0px;
    -webkit-margin-end: 0px;
    font-weight: bold;
    width: 170px;
    height: 34px;
    background-position: 0 0;
}
</style>