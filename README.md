# Dino Hacker 🤖🦖

O **Dino Hacker** é um projeto de automação física que "joga" o famoso jogo do dinossauro do Google de forma totalmente autônoma! Usando sensores de luz (LDRs) e servomotores controlados por um Arduino, o sistema detecta obstáculos na tela e faz o dinossauro pular no momento certo.

A mágica acontece sem qualquer interferência no código do navegador ou do jogo. Em vez disso, o projeto simula fisicamente o ato de pressionar a tecla *espaço*, exatamente como faria um jogador humano — só que mais rápido e preciso!

## Como funciona

- Dois sensores de luz (LDRs) são posicionados estrategicamente em frente à tela, monitorando a região por onde os obstáculos passam.
- Quando um obstáculo se aproxima, a luminosidade detectada pelos sensores muda.
- O Arduino lê esses valores analógicos e, ao detectar essa mudança, aciona dois servomotores.
- Os servos são responsáveis por pressionar fisicamente a tecla de pulo (geralmente o espaço), fazendo o dino desviar dos obstáculos.

## Componentes utilizados

- 1 Arduino (UNO, Nano, etc.)
- 2 sensores LDR
- 2 resistores (para formar divisores de tensão com os LDRs)
- 2 servomotores (ex: SG90)
- Jumpers e protoboard

## Código
O código lê constantemente os valores dos sensores A0 e A1 e, se ambos estiverem abaixo de certos limites (indicando um obstáculo), os servos são acionados para moverem 20 graus (simulando o pulo). Em seguida, eles voltam à posição inicial.

Video sobre o projeto

https://www.youtube.com/watch?v=w2mFwqaoyVY&ab_channel=SobreCorrente
