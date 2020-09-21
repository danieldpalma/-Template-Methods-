# Padrão Template Methods

* Pattern Name and Classification
  - Name: Template Methods
  - Classification: Comportamental

* Intent
  - Facilitar a alteração de comportamente do algoritmo sem precisar alterar a estrutura inteira.

* Motivation
  - O Template Method permite criarmos uma classe pai com métodos abstratos onde as classes filhos alteram esse método para um comportamento específico da mesma.

* Applicability
  - O Template Method deve ser utilizado em aplicações que possuem estrutura hierárquica e um algoritmo que pode ser divido em etapas.

* Structure

![](https://miro.medium.com/max/866/1*fyEAfGmdfL9RPiz5ua_HCA.png)

* Paticipants
  - ApplicantionClassOne/ApplicationClassTwo:
    - Declara interface para objetos da composição
    - Implementa comportamentos padrão comuns para todas as classes
    - Declara uma interface para acessar e gerenciar componentes filho
  - FrameworkClass:
     - Define o Template Method que é responsável por chamar os demais métodos.;
    - Especifica os métodos abstratos das etapas de execução.

* Sample Code
  - [Código](https://repl.it/repls/OpenStaticMass#Main.java)
  - Para demonstrar o padrão Template Methods, foi tentando fazer um programa em que se escolhe a versão de uma carro entre Joy, LT e LTZ e então é mostrado os opcionais presentes em cada versão.
