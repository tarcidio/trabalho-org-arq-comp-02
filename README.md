# Trabalho 02 SCC0902 Organização e Arquitetura de Computadores:

## Autores:

* Tarcídio Antônio Júnior - 10748347
* Jade Bortot de Paiva - 11372883
* Gabriel Barbosa de Oliveira - 12543415
* Luís Filipe Vasconcelos Peres - 10310641

## Introdução

  A disciplina de Organização e Arquitetura de Computadores é crucial para profissionais de tecnologia da informação. Ela oferece uma compreensão sólida do funcionamento interno dos computadores e seus componentes, sendo fundamental para o desenvolvimento de softwares e hardwares eficientes. Além disso, o estudo dessa disciplina ajuda a solucionar problemas em sistemas computacionais, identificando falhas de desempenho e segurança e encontrando soluções apropriadas.

## Objetivo do trabalho
  
O objetivo deste trabalho é implementar e simular um processador x32 RISC-V em pipeline usando o Logisim. A técnica de pipeline é empregada para otimizar o desempenho do processador, dividindo as instruções em estágios e executando-os simultaneamente. Compreender o funcionamento do pipeline e seus componentes básicos é fundamental para compreender a arquitetura de um computador.

Além da implementação, serão realizados testes utilizando instruções básicas para verificar a funcionalidade do processador simulado. O trabalho também busca ser um recurso educativo, fornecendo material para os futuros alunos da disciplina de Organização e Arquitetura de Computadores.
  
## Ferramentas

Foi utilizado o simulador Logisim-ITA, uma ferramenta gratuita de simulação de circuitos digitais. Ele possui uma interface gráfica intuitiva que permite a criação e teste de circuitos combinacionais e sequenciais. O Logisim-ITA é popular entre estudantes, educadores e entusiastas da eletrônica digital devido à sua facilidade de uso. Possui uma ampla biblioteca de componentes lógicos, como portas, flip-flops e registradores, que podem ser arrastados e soltos na interface. Além disso, o Logisim-ITA oferece recursos de simulação e modularização, permitindo a criação de subcircuitos reutilizáveis para facilitar a construção de circuitos mais complexos.
  Para usar o Logsim, siga as instruções abaixo:
 1. Acesse o site https://logisim.altervista.org/
 2. Role até o fim da página
 3. Clique em "DOWNLOAD"
 4. Em segundos, o arquivo .exe do Logsim será baixado
 5. Vá até a pasta de "Downloads" e abra o arquivo baixado
    Também foi usado como base o livro "GUIA PRÁTICO RISC-V: ATLAS DE UMA ARQUITETURA ABERTA": livro abrangente que explora a arquitetura RISC-V de forma prática. Ele apresenta os conceitos fundamentais e a implementação dessa arquitetura de processador aberta. Exploramos principalmente a [página 17 e 18](https://github.com/tarcidio/trabalho-org-arq-comp-02/blob/main/instrucoes_risc_v.pdf), onde consta as instruções.
    
## Discussão e resultados

Para facilitar a discussão de todo o trabalho, fizemos vídeos que descrevem melhor os componentes e a implementação. Segue:

* [Vídeo 01: Introdução ao Logisim](https://www.youtube.com/watch?v=ZZsND2eOAwo)
* [Vídeo 02: Subcircuitos usados](https://www.youtube.com/watch?v=1rVrc5WXauU)
* [Vídeo 03: Explicação da implementação](https://www.youtube.com/watch?v=ZJE4mW0OjPg)
* [Vídeo 04: Desafios](https://www.youtube.com/watch?v=-ZBtMzy1AJU)

Neste trabalho, implementamos os seguintes subcircuitos:
* banco_de_registradores.circ: circuito que representa o conjunto de registradores do processador;
* conversor_32_23.circ: como a memória RAM do logisim só é endereçada com 24 bits, não podemos usar os 32 bits da arquitetura. Para converter, modularizamos um pequeno circuito;
* detector_tipo_instrucao.circ: subcircuito usado na unidade de controle para identificar o tipo da instrução;
* immediate_generator.circ: circuito que determina o valor imediado da instrução;
* unidade_controle.circ.circ: figura central do processador, é quem maestra os sinais de controle;
* unidade_controle_ula.circ: determina qual operação deve ser feita na ULA;
* unidade_logica_aritmetica.circ: componente que faz os cálculos necessários para a instrução;
* monociclo.circ: primeiro componente principal. Para construir a pipeline, fizemos a monociclo primeiro;
* pipeline.circ: componente principal o qual é o objetivo do trabalho.

Implementamos as seguintes instruções:
* Tipo R: add
* Tipo I: lw
* Tipo S: sw
* Tipo B: beq
* Tipo J: jal
  
O código que está no "MEMORIA_INSTRUCOES" é:

0x00: lw t0, 4(zero)
0x04: lw t1, 8(zero)
0x08: add zero, zero, zero
0x12: add zero, zero, zero
0x16: add t2, t1, t0
0x20: add zero, zero, zero
0x24: add zero, zero, zero
0x28: sw t2, 16(sp)
0x32: beq t3, zero, 40
0x68: j  ra, -0x68 (111111111111110011000)

Veja melhora no arquivo "[instrucoes.txt](https://github.com/tarcidio/trabalho-org-arq-comp-02/blob/main/instrucoes.txt)".

[GIF]

## Desafios
  Dentre os desafios enfrentados, podemos citar:
  1. Fazer subcircuitos que não sabiamos como funcionava de fato. O principal exemplo foi o banco de registradores;
  2. Manipular os fios de forma que todo o circuito fosse o mais didático possível;
  3. Sincronizar o clock para que resolvesse o problema da dependencia estrutural

## Pontos de melhoria para os próximos alunos

1. Implementar outras instruçoes da arquitetura;
2. Implementar técnicas que resolvam melhor o problema de dependência de dados;
3. Implementar cache

## Quer me ajuda?

Se encontrar erros neste projeto, por favor, faça um pull ou nos chame para conversar! Adoraríamos melhorar este trabalho para os próximos alunos. Se implementar uma melhoria (instruções, forwarding, cache, dentre outras), avise nos! Anexaremos o link do seu trabalho neste git hub.


Vamos melhorar o aprendizado desta disciplina ;)

---

<sup>Instituto de Ciências Matemáticas e de Computação (ICMC) - Universidade de São Paulo (USP)</sup>

