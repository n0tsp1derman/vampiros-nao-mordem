# vampiros-nao-mordem
projeto de uma visual novel interativa para a Apple Developer Academy, contando um pouquinho sobre a minha rotina :)

# Vampiros não mordem (eles fazem faculdade)

É uma visual novel interativa onde é possível acompanhar a rotina de Yasmin, uma universitária comum que definitivamente não é um vampiro disfarçado. Mas se hipoteticamente falando ela fosse um, seu maior problema não seria nem ter medo de sol e não poder usar prata: e sim o caos da rotina dela mesmo sendo um ser imortal. 

São tantas coisas pra fazer, em tão pouco tempo, e fingir que ela não tem 400 anos de idade é bem complicado… Ajude Yasmin a escolher o que fazer durante o seu dia, e conheça um pouco dela enquanto o tempo vai passando!

## Como surgiu a ideia?

Eu tenho muitos interesses e hobbies, o que faz com que 1. eu sempre esteja ocupada 2. eu nunca saiba como me definir em poucas palavras. Então pra que escolher um aspecto da minha personalidade se eu posso fazer um panorama geral? E nada melhor para isso do que contar minha rotina corrida de estudante. 

Somei essa primeira ideia com outros dois pontos. O primeiro é que sempre tive muita vontade de fazer uma visual novel, e queria me aprofundar mais em pixel art para deixar o app com essa carinha de jogo. O segundo é que entre meus amigos da faculdade, existe uma piada interna de que eu sou um vampiro disfarçado. Afinal de contas, minha palidez, jeito de me vestir e amor por tudo que é gótico acabam corroborando um pouco pra isso… Achei que essa piadinha daria um tom mais engraçado e diferente para a narrativa, então criei essa história sobre um vampiro que, ao contrário do Edward Cullen, faz faculdade ao invés de Ensino Médio. 

## E como meu projeto veio à vida?

### Narrativa

A primeira coisa que eu fiz foi um pequeno moodboard com referências pra pixel art e um fluxograma para destrinchar todas as telas e assets que eu teria que fazer, além de usar ramificações a partir de escolhas do jogador para trazer essa lógica de visual novel. Nem preciso dizer que tive que diminuir muito meu escopo ao longo do projeto rs…. 

![Screenshot 2025-04-28 at 15.12.56.png](attachment:9bca002e-4cf3-4210-9217-d8ec83c0655d:Screenshot_2025-04-28_at_15.12.56.png)

![Screenshot 2025-04-28 at 15.14.28.png](attachment:15b5784d-f3d2-4ec8-b80e-a524e1929f06:Screenshot_2025-04-28_at_15.14.28.png)

![Screenshot 2025-04-28 at 15.22.15.png](attachment:3c5e6363-d332-4625-b753-6a8713993cae:Screenshot_2025-04-28_at_15.22.15.png)

Então, comecei a pensar em uma narrativa voltada para a minha rotina. Dividi meu fluxograma geral em 3 "fases” a partir de período do dia (manhã, tarde e noite) e montei um roteiro com todo o diálogo, texto introdutório e as ações que aconteceriam no jogo inteiro. Foquei em frases curtas que não são maçantes de ler e se encaixam em um loop de animação curto. 

### Design

Então fiz uma lista de requisitos com tudo que eu precisava fazer e aprender, e comecei a trabalhar nos meus assets no Aseprite. Usei uma paleta de cores do Lospec chamada Ressurect para limitar minhas escolhas e defini meu frame máximo para 1920x1080, para não ter problemas com o posicionamento dos assets.  Milagrosamente, não demorei para conseguir um estilo que me agradasse, e aos poucos fui fazendo a parte do design. Assim que tinha uma base pronta, montei um protótipo de alta fidelidade no Figma para me guiar, e fiz todos os assets de apoio por lá também. 

Consegui refinar bastante meu processo e aproveitei para cortar alguns caminhos que eu sabia que teria dificuldade. Por exemplo, ao invés de colocar todo o meu texto pelo Playgrounds, optei por salvar como imagem quando eu sabia que eles não iriam sofrer alterações, o que facilitou muito na hora do posicionamento. 

![Screenshot 2025-04-29 at 15.26.50.png](attachment:f0f33dff-69e5-4bc8-adb8-1bf3704c508a:Screenshot_2025-04-29_at_15.26.50.png)

### Programação

Então, enquanto produzia o resto dos assets, comecei a aprender a programar no Swift Playgrounds. Com a ajuda dos mentores e dos meus amigos (e do ChatGPT), aos poucos fui desenvolvendo uma base de código. Escolhi propositalmente mecânicas que fossem se repetir ao longo da visual novel, como passar telas, apertar botões e iniciar loops de animação, o que me permitiu fazer um jogo um pouco mais longo e focar em fazer assets diferentes ao invés de me aventurar em algo que eu não me sentia tão segura, como a programação. 

Separei cada tela principal em files .swift diferentes para deixar meu código mais organizado.

![Screenshot 2025-04-29 at 15.28.32.png](attachment:0a4ba37b-4ea9-4dae-b970-390ecf267e7f:Screenshot_2025-04-29_at_15.28.32.png)

O esqueleto da minha visual novel é bem clássico, com um botão que vai passando diálogos com um contador que, após exaurir todo o texto, automaticamente avança para a próxima tela usando NavigationStacks. Usei H/V/ZStacks para organizar todos os meus assets de modo a parecer uma visual novel. Além disso, adaptei um loop de animação feito para o SwiftUI que não precisava do uso do SpriteKit e usei a base do código Explode passado pelos mentores para uma parte da narrativa. 

Tive muita dificuldade principalmente com o posicionamento e com a ordem de execução de cada uma de minhas ações a partir dos botões que eu criei, mas depois que entendi melhor a lógica do Swift e com a ajuda dos amigos e mentores consegui resolver. 

No final, após resolver os principais bugs e problemas, usando o AVFoundation adicionei um áudio de diálogo do jogo Animal Crossing para representar minha fala, e adicionei a música Aruarian Dance do artista Nujabes. 

---

# Video

[vampiros nao mordem.mp4](attachment:67a2b2ca-b99a-4015-bcfe-254ab7e1a31a:vampiros_nao_mordem.mp4)

---

---

# Assets

![cena 1.png](attachment:9b976040-1333-40d2-af4b-f7299b0e55bf:cena_1.png)

![cena 2.png](attachment:9495a642-e99a-4a73-980c-99d090534fe2:cena_2.png)

![fundo_estante.png](attachment:6ee6a666-287a-4ef3-8cc7-643f143f1a21:fundo_estante.png)

![fundo_UFPR.png](attachment:f2ce4e4b-0bbc-4b8c-a4a4-ed4b6de7506a:fundo_UFPR.png)

![por do sol.gif](attachment:c122e5e8-20b8-4264-80a6-1127434bfbd7:por_do_sol.gif)

![ligeirao loading screen.gif](attachment:a6bd81e1-d674-4793-a9a1-57b80d407284:ligeirao_loading_screen.gif)

![mimir.gif](attachment:677bf8ee-a4b0-4f28-a287-e1a48a34576e:mimir.gif)

![jogos.png](attachment:59583360-6894-42b3-a663-8e7a17d8cf52:jogos.png)

---
