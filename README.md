# Trabalho 02 SCC0902 Organização e Arquitetura de Computadores:

## Autores:

* Tarcídio Antônio Júnior - 10748347
* Jade Bortot de Paiva - 11372883
* Gabriel Barbosa de Oliveira - 12543415
* Luís Filipe Vasconcelos Peres - 10310641

## Introdução

  A disciplina de Organização e Arquitetura de Computadores é crucial para estudantes e profissionais de tecnologia da informação. Ela oferece uma compreensão sólida do funcionamento interno dos computadores e seus componentes, sendo fundamental para o desenvolvimento de softwares e hardwares eficientes capazes de executar operações complexas de forma rápida e precisa. Além disso, o estudo dessa disciplina também ajuda a solucionar problemas em sistemas computacionais, identificando falhas de desempenho e segurança e encontrando soluções apropriadas.

## Objetivo do trabalho
  
  O objetivo deste trabalho é implementar e realizar a simulação do processamento em pipeline de um processador RISC-V utilizando a ferramenta Logisim, simulando algumas instruções e servindo como material educativo para os próximos alunos da disciplina de Organização e Arquitetura de Computadores. 
  Pipeline é uma técnica de otimização amplamente utilizada na arquitetura de computadores, que visa aumentar a eficiência do processador dividindo as instruções em estágios distintos e executando-os simultaneamente. Entender seu funcionamento, desde de conhecer os componentes básico (banco de registradores, unidade de controle, unidade lógica e aritmética, dentre outros) até como se desenvolve a sincronia entre cada um dos estágios (busca de instrução, decodificação, busca de operandos, execução e escrita de resultados) é a base da compreensão de como um computador funciona. 
  Para facilitar a ilustração, lançamos mão de testes de algumas instruções básicas implementadas a fim de verificar sua corretude e funcionalidade. Desta maneira, o material poderá ser útil para alunos no futuro servindo como ferramenta de aprendizado.
  
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

Descrição: Neste vídeo, explicamos sobre como baixar o projeto e como usar o Logisim.

[Vídeo 02: Subcircuitos usados]([URL]https://www.youtube.com/watch?v=1rVrc5WXauU)

Descrição: Neste vídeo, explico sobre os subcircuitos usados no projeto.

[Vídeo 03: Explicação da implementação](https://www.youtube.com/watch?v=ZJE4mW0OjPg)

Descrição: Neste vídeo, explicamos a implementação e o trabalho de fato

[Vídeo 04: Desafios](https://www.youtube.com/watch?v=-ZBtMzy1AJU)
Descrição: Neste vídeo, damos sugestões de como melhorar o projeto com alguns desafios.

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

