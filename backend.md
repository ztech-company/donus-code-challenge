# Desafio de Backend

## Sobre o Desafio

Seu objetivo é criar um serviço que exponha uma API REST e possua duas funcionalidades básicas.

#### 1. Criar um filme
Criar uma rota onde seja possivel criar um filme. Um filme deve contar as seguintes propriedades: Nome do Filme, Data de Lançamento, Nivel de Censura (CENSURADO ou SEM_CENSURA), Direção e Elenco. O Elenco deve ser uma lista de atores. 

Regras: 
* Não podem existir dois filmes com nomes iguais.
* Um filme não pode ter mais do que 10 atores.
* A lista de atores deve ser informada no momento de criação de um filme.

#### 2. Buscar lista de filmes
Criar uma rota que seja possível listar os filmes utilizando como filtro o nível de Censura (CENSURADO ou SEM_CENSURA).


## Regras do Desafio
* Para expôr suas API's utilize de preferência um framework Web simples e leve. O objetivo do teste não é saber se você sabe utilizar um framework web, mas sim se você utiliza boas práticas de desenvolvimento.
* Não utilize boilerplates, gostamos de ver como o desenvolvedor organiza seu código.
* Fique a vontade para escolher o banco de dados que achar melhor.
* Dockerize sua aplicação. Isso facilitará para quem está corrigindo seu teste.

## Como avaliaremos?
Avaliaremos o desafio baseado nos aspectos abaixo:
* Seu código é construído utilizando práticas de DDD ( Domain Driven Design ) como Domínios, Serviços, Repostórios e etc.
* Seu código aplica boas práticas de desenvolvimento como SOLID e DRY.
* Seu código possui testes automatizados incluindo testes unitários, testes integrados e testes end-to-end.
* Seu código retona códigos de erros claros e descritivos (Tratamento de Erros)