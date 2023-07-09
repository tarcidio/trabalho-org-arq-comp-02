# Trabalho 02 SCC0902 Organização e Arquitetura de Computadores:

## Autores:

* Tarcídio Antônio Júnior - 10748347
* Jade Bortot de Paiva - 11372883
* Gabriel Barbosa de Oliveira - 12543415
* Luís Filipe Vasconcelos Peres - 10310641

## Introdução

  A disciplina de Organização e Arquitetura de Computadores é crucial para profissionais de tecnologia da informação. Ela oferece uma compreensão sólida do funcionamento interno dos computadores e seus componentes, sendo fundamental para o desenvolvimento de softwares e hardwares eficientes. Além disso, o estudo dessa disciplina ajuda a solucionar problemas em sistemas computacionais, identificando falhas de desempenho e segurança e encontrando soluções apropriadas.

## Objetivo do trabalho
  
<t>O objetivo deste trabalho é implementar e simular um processador RISC-V em pipeline usando o Logisim. A técnica de pipeline é empregada para otimizar o desempenho do processador, dividindo as instruções em estágios e executando-os simultaneamente. Compreender o funcionamento do pipeline e seus componentes básicos é fundamental para compreender a arquitetura de um computador.

Além da implementação, serão realizados testes utilizando instruções básicas para verificar a funcionalidade do processador simulado. O trabalho também busca ser um recurso educativo, fornecendo material para os futuros alunos da disciplina de Organização e Arquitetura de Computadores.
  
## Ferramentas

  Para elaboração, utilizou-se o simulador gratuito Logisim-ITA: ferramenta de simulação de circuitos digitais utilizada para projetar e testar a lógica digital. Ele permite a criação de circuitos combinacionais e sequenciais usando uma interface gráfica intuitiva, o que o torna uma opção popular para estudantes, educadores e entusiastas da eletrônica digital. Tal ferramenta possui uma vasta biblioteca de componentes lógicos (desde portas lógicas, passando por flip flops, até registradores e memória RAM) os quais podem ser utilizados "arrastando e soltando". Por fim, Logisim é útil também por conta da sua capacidade de simular circuitos e compactá-los de forma a modularizá-los, criando subcircuitos reutilizáveis, facilitando a construção de circuitos mais complexos.
  Para usar o Logsim, siga as instruções abaixo:
 1. Acesse o site https://logisim.altervista.org/
 2. Role até o fim da página
 3. Clique em "DOWNLOAD"
 4. Em segundos, o arquivo .exe do Logsim será baixado
 5. Vá até a pasta de "Downloads" e abra o arquivo baixado
    Também foi usado como base o livro "GUIA PRÁTICO RISC-V: ATLAS DE UMA ARQUITETURA ABERTA" (complementar um pouco)

## Discussão e resultados


[Vídeo 01: Introdução ao Logisim](https://www.youtube.com/watch?v=ZZsND2eOAwo)

[Vídeo 02: Subcircuitos usados](https://www.youtube.com/watch?v=1rVrc5WXauU)

[Vídeo 03: Explicação da implementação](https://www.youtube.com/watch?v=ZJE4mW0OjPg)

[Vídeo 04: Desafios](https://www.youtube.com/watch?v=-ZBtMzy1AJU)


video:
explicar o que são os arquivos
como abrir
como olhar os subcircuitos
como carregar dados e instruções
como fazer o clock funcionar para que as isntruções sejam acessadas
explicar o detalhe da incrementacao do contador

explicar que inicialmente fizemos os subcircuitos e explicar cda um deles resumidadmente para fazer o monociclo e então deposi fazer os pipeline colocando os registradores intermediarios
explicar inicialmente que o circuito está no arquivos pipiline.circ
explicar cada um dos compoenentes
explicar quais instruções foram implementadas
explicar qual codigo está no arquivo memoria instrucoes
explicar que fizemos u mjvideo simples
mostrar um gifizinho funcionando
  
## Desafios
  Via de regra, o trabalho foi a aplicação do que foi muito bem ensinado já em sala de aula. Portanto, os desafios foram pontuais. O primeiro deles foi a utilização da chamada ao sistema para alocação de memória que até então não se tinha usado. O segundo desafio foi separar o código em funções. Este levou mais tempo, pois foi necessário revisitar o código após uma semana e isso fez com que o grupo se esquecesse, mesmo com os devidos comentários, do que cada comando no código fazia. Por fim, o grupo também tentou separar as funções em um arquivo a parte para incluí-lo depois, mas não foi possível, pois o simulador não permite. 

faer subcircuios que noa sabiamos (banco de registadores)
arrastas os fios para que fosse o mais compreensiveis possivel
corrigir problemas no clock para que resolvesse o problema da dependnecia estrutural (escrita e dps leitura)


# Pontos de melhoras para os próximos alunos

implementar outras instruçoes
fazer o forword
implementar cache

fazer video para desafios explicando um pouco

se encntrar erros ou fizer uma melhoria (implementar outas instruções, forward ou cachae), avise me que anexarei o link do git hub do projeto neste git hub

vamso melhorar oaprendizado de org arq comop

---

<sup>Instituto de Ciências Matemáticas e de Computação (ICMC) - Universidade de São Paulo (USP)</sup>

