# Film Wars

### Introdução
Este projeto utiliza a [Star Wars API (SWAPI)](https://swapi.dev/) para desenvolver uma aplicação baseada em nuxt 3, que será composta por três páginas principais: 
- Página inicial para a busca de filmes
- Detalhe do filme: será exibido detalhes de um filme selecionado
- Informações do personagem: será exibido detalhes de um personagem selecionado

### Helpers

Como a API não tem imagens, use a [imagem gerada de um gerador de imagens](https://picsum.photos/200/300). Veja a [doc dele aqui](https://picsum.photos/)

#### Utils
- [Documentação da api](https://swapi.dev/)
- [Listagem de filmes](https://swapi.dev/documentation#films)
- [Listagem de pessoas](https://swapi.dev/documentation#people)

#### Design
- Fonte: Open Sans
- Tamanho max do conteúdo: 920px

#### Cores

| Color | Hex |
| ----- | --- |
| Background | ![#161616](https://via.placeholder.com/10/161616?text=+) #161616 |
| Bg Header | ![#202020](https://via.placeholder.com/10/202020?text=+) #202020 |
| Primary Color | ![#FFCC02](https://via.placeholder.com/10/FFCC02?text=+) #FFCC02 |
| Bg Input, Bg Card | ![#323232](https://via.placeholder.com/10/323232?text=+) #323232 |
| Text | ![#FFFFFF](https://via.placeholder.com/10/FFFFFF?text=+) #FFFFFF |
| Button color | ![#000000](https://via.placeholder.com/10/000000?text=+) #000000 |

### Home (Listagem de Filmes)
A página inicial terá uma listagem de filmes da saga Star Wars, onde cada filme exibirá as seguintes informações em cada item da lista:

- Imagem de capa
- Título do Filme
- Descrição

No caso de um dos cards ser clicado, o usuário será levado para a página de detalhe de um filme, conforme o id selecionado.

![home](https://github.com/vinimw/FilmWars/blob/main/images/home-sketch.png?raw=true)

### Detalhe de um filme

Ao ser clicado ou acessado a url de detalhe de um filme, deve ser mostrado alguns detalhes do filme selecionado como:
- Imagem de capa (pode ser randomica)
- Título do filme (title)
- Descrição (opening_crawl)
- Diretor (director)
- (release_date) para a data após o conteúdo do diretor
- Episódio (episode_id)
- Produção (producer)

Além disso será mostrado a lista de personagens que fazem parte do filme selecionado, pode ser  mostrado de forma simples limitando a 4 ou como preferir.

Ao clicar para ver mais sobre aquele personagem, o usuário será levado para a página de detalhe de um personagem.

![movie-detail](https://github.com/vinimw/FilmWars/blob/main/images/movie-detail-sketch.png?raw=true)


### Detalhe de um personagem

Nessa página será mostrado informações sobre o personagem como:

- Nome (name)
- Cor dos olhos (eye_color)
- Cor do cabelo (hair_color)
- Altura (height)
- Listagem de filmes no quais ele participou (films)
