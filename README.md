# Projeto Tetris

Este projeto foi desenvolvido utilizando como base o repositório de Michael Káren, feito em Javascript.

Foram utilizados os elementos:
- **HTML**: Para a composição da tela inicial do jogo;
- **CSS**: Estilização da tela, fonte e do botão de Play;
- **Javascript**: Comportamento do jogo. Para isso foram definidas algumas classes que realizariam estes comportamentos:
  - **Board**: Responsável pela lógica e comportamento das peças, como a inicialização, reset, desenho das peças, movimentação de queda, limpeza das linhas quando há pontuação, validações de colisão, rotação e pontuação;
  - **Constants**: Configuração das regras de jogo, como definição das colunas e linhas do board, cores, formas matriciais das peças, teclas utilizadas, definição da pontuação e da velocidade da queda das peças por nível;
  - **Main**: Definição da inicialização do jogo, utilização do canvas para gerar os elementos 2D, atualização da pontuação, inicialização, movimentação, animação, pausa  e game over das peças; 
  - **Piece**: Lógica das peças, cosntrutores para sua geração e forma de movimentação na tela, além da função que gera formas aleatórias;
- A tela inicial de jogo terá essa aparência:

![Main](https://github.com/lucasbriz/projeto-tetris/blob/main/assets/main.JPG)

# Funcionamento

- O jogo tem uma premissa simples; começamos com um quadro em branco e, ao dar o _Play_, serão geradas peças, chamadas de Tetrominos, de forma aleatória, baseadas em suas características, identificadas como I, J, L, O, S, T, e Z:

![Tetrominos](https://github.com/lucasbriz/projeto-tetris/blob/main/assets/tetrominos.JPG)

- Cada peça irá começar a cair e o jogador pode movê-la para os lados utilizando as setas direita e esquerda do teclado e a seta para cima, para rotacionar a peça. Quando atingir outra peça na horizontal, ela permanecerá imóvel e outra peça será gerada. Então, o jogador deve encaixar as peças a fim de que ele complete uma linha inteira e, com isso, ganhar pontos.
- O jogo será encerrado quando qualquer peça atingir o topo da tela.

![Game-Over](https://github.com/lucasbriz/projeto-tetris/blob/main/assets/game-over.JPG)
