<h2>API: PotterDB<h2>

<h1 align="center"><img src= "https://user-images.githubusercontent.com/101807045/229957740-54ce8e39-fdef-4c6e-9a9d-3ce9f55fa2ae.png" heigth="250px" width="250px"/></h1>
<p align="center">
<img src="http://img.shields.io/static/v1?label=FUNCIONALIDADE&message=APRESENTA%20DADOS%20REFERENTES%20AO%20MUNDO%20DO%20HARRY%20POTTER: PERSONAGENS, FILMES%20E%20LIVROS&color=yellow&style=for-the-badge"/>
</p>

 <details open="sumarioo">
 <summary><b>Sumário:</summary></b>
  
- [ Desenvolvedores ](#Desenvolvedores)
- [ Funcionalidades ](#funcionalidades)
- [ URL da Documentação ](#1)
- [ URL de Acesso a API ](#2)
- [ Métodos Disponíveis ](#3)
- [ Filtragem ](#5)
- [ Atributos soclitados por cada método ](#4)

</details>

## :computer: Desenvolvedores
**Desenvolvido por:** Beatriz Pereira Campos e Emilynn Nogueira Calixto Zabala; <br>
**Turma:** 3ºDS;

## :hammer: Funcionalidades
<p Align="justify"> O tema central da nosso projeto é a saga de “Harry Potter”, onde trabalhamos com o intuito de desenvolver uma aplicação diretamente focada em atrair os grandes espectadores e fãs dessa saga, procurando levar informações e trazer diversas funcionalidades, exclusividades e entretenimento ao usuário. A implementação da API, tem como principal funcionalidade retornar dados referentes ao tema, como: personagens, livros e filmes. </p>

## 🔗 URL da Documentação
https://github.com/danielschuster-muc/potter-db

## 🔗 URL de Acesso a API
https://api.potterdb.com/
 
 
## 📒 Métodos Disponíveis
Para acessar os dados das APIs é necessário fazer um GET solicitando os seguintes endpoints.
Vamos chamar este GET através de uma linha de comando, como por exemplo: (https://api.potterdb.com/v1/characters/harry-potter).
 
<details close="metodo1">
<summary><b>Livros</summary></b>
 
- `/v1/books`
: Este método irá obter recursos hospedados no servidor e retornará a lista de todos os livros.

- `/v1/books/:slug`
: Este método irá obter recursos hospedados no servidor e retornará a lista de livros específicos.

</details>
 
<details close="metodo2">
<summary><b>Capítulos</summary></b>
 
- `/v1/books/:chapters`
: Este método irá obter recursos hospedados no servidor e retornará a lista de todos os capítulos de um certo livro.

- `/v1/books/:chapters/:slug`
: Este método irá obter recursos hospedados no servidor e retornará a lista de um capítulo específico de um livro específico.

</details>
 
<details close="metodo3">
<summary><b>Personagens</summary></b>
 
- `/v1/characters`
: Este método irá obter recursos hospedados no servidor e retornará a lista de todos os personagens.

- `/v1/characters/:slug`
: Este método irá obter recursos hospedados no servidor e retornará a lista de personagens específicos.

</details>
 
<details close="metodo4">
<summary><b>Filmes</summary></b>
 
- `/v1/movies/`
: Este método irá obter recursos hospedados no servidor e retornará a lista de todos os filmes.

- `/v1/movies/:slug`
: Este método irá obter recursos hospedados no servidor e retornará a lista de filmes específicos.
 
</details>

## :pushpin: Filtragem
 
- `/v1/characters?filter[name_cont_any] = name`
: Este método de organização irá filtrar os resultados retornando apenas os caracteres buscado por um nome específico.

- `/v1/characters?sort = name`
: Neste método de organização pode-se classificar os resultados por um campo específico.

- `/v1/characters?page[number = 10]&page[size = 20]`
: Este método de organização irá filtrar os resultados retornando apenas a página desejada e a quantidade de resultados que foram escolhidos.

 
## 📄  Atributos solicitados por cada Método
<details close="atributos1">
<summary><b>Livros</summary></b>

- `slug`
: O slug é um parâmetro que faz parte da URL, sendo utilizado como identificador. Nesse caso, ele identifica o livro, pelo seu ID.

- `title`
: O título deste livro.
 
- `summary`
: O resumo deste livro.
 
 - `author`
 : O autor do livro.
 
 - `realese_date`
 : Data na qual o livro foi lançado.
 
 - `pages`
 : O número de páginas deste livro.
 
 - `order`
 : A ordem cronológica deste livro dentro da saga de Harry Potter (ex: 1.Harry Potter e a pedra filosofal; 2.Harry Potter e a câmara secreta...);
 
 - `wiki`
 : Link de direcionamento para página específica deste livro.
</details>
 
<details close="atributos2">
<summary><b>Capítulos</summary></b>
  
  - `slug`
  : O slug é um parâmetro que faz parte da URL, sendo utilizado como identificador. Nesse caso, ele identifica um capítulo específico do livro.

 - `title`
  : O título deste capítulo.
  
  - `summary`
  : O resumo deste capítulo.
  
  - `order`
  : A ordem cronológica deste capítulo dentro do livro (ex: Capítulo 1, Capítulo 2...);
  
</details>
 
 <details close="atributos3">
 <summary><b>Personagens</summary></b>
  
  - `slug`
 : O slug é um parâmetro que faz parte da URL, sendo utilizado como identificador. Nesse caso, ele identifica um personagem específico, pelo seu ID.
 
 - `Name`
 : O nome deste personagem.
   
 - `Born`
 : A data de nascimento deste personagem.
  
 - `gender`
 : O gênero deste personagem.
   
 - `image`
 : Um link para uma imagem deste personagem.
   
 - `wiki`
 : Link de direcionamento para página específica deste personagem.
</details>
 
  <details close="atributos4">
 <summary><b>Filmes</summary></b>
  
  - `slug`
 : O slug é um parâmetro que faz parte da URL, sendo utilizado como identificador. Nesse caso, ele identifica um filme específico, pelo seu ID.
 
 - `title`
 : O título deste filme.
   
 - `summary`
 : O resumo deste filme.
   
 - `trailer`
 : Um link para o trailer deste filme em específico.
   
 - `wiki`
 : Link de direcionamento para página específica deste filme.
</details>
 
 
