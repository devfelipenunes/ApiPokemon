# PokeAPI

## Consumindo Api de Pokemon

Nesse projeto consumir a api pokeapi, onde consigo capiturar o nome ou o numero do pokemon desejado, e assim retornar o resultado esperado.

## Site

Teste o consumo da API [ApiPokemon](https://devfelipenunes.github.io/ApiPokemon/)

![video](https://user-images.githubusercontent.com/81275678/158929763-d8f174b4-88ab-48d2-83e8-8bb997407b77.gif)

## Função DataNascimento()

Essa função pega o valor do input do date e divide ele em dia/mes/ano.
Faz soma do ultimo numero de cada variavel (dia/mes/ano).
Exemplo - 22/03/1998 seria então 238

````
function dataNascimento(){
  var data = document.getElementById("dataNascimento").value
  data = data.replace(/\//g, "-")
  var data_array = data.split("-")
  
  var dia = data_array[2]
  var mes = data_array[1]
  var ano = data_array[0]

  var pokemonData = dia.slice(-1) + mes.slice(-1) + ano.slice(-1)

  startApp(pokemonData)
}
````

Assim fazendo a busca na api do numero na pokedex do pokemon

![videoDois](https://user-images.githubusercontent.com/81275678/162875552-6e2a56f7-0323-49d6-b67d-08f75214b67b.gif)



