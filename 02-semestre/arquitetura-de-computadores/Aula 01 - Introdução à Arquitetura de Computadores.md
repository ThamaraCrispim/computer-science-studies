# Aula 01 - Introdução à Arquitetura de Computadores

## Conteúdos abordados

Nesta aula foram estudados os conceitos introdutórios de Arquitetura de Computadores, a evolução histórica dos computadores, os principais componentes de um sistema computacional, o modelo de Von Neumann, o funcionamento básico da CPU, níveis hierárquicos e alguns conceitos de desempenho.

---

## 1. O que é Arquitetura de Computadores?

A Arquitetura de Computadores estuda como os componentes de um computador são organizados e como trabalham em conjunto para executar instruções, processar informações e armazenar dados.

De forma simplificada:

**Computador = Processador + Memória + Entrada/Saída + Armazenamento**

O estudo da arquitetura permite compreender:

- Como o computador funciona internamente;
- Como as informações são processadas;
- Como os dados são armazenados;
- Como hardware e software se relacionam;
- Como os computadores evoluíram;
- Como identificar problemas de desempenho e gargalos.

---

## 2. Hardware e Software

### Hardware

É a parte física do computador.

Exemplos:

- Processador;
- Memória RAM;
- Placa-mãe;
- HD e SSD;
- Teclado;
- Mouse;
- Monitor;
- Placa de vídeo.

### Software

É a parte lógica do computador, formada pelos programas e instruções executados pelo hardware.

Exemplos:

- Sistemas operacionais;
- Aplicativos;
- Programas;
- Drivers;
- Utilitários.

Hardware e software trabalham em conjunto para permitir o funcionamento do sistema computacional.

---

## 3. Computadores analógicos e digitais

### Computadores analógicos

Trabalham com grandezas ou sinais contínuos.

### Computadores digitais

Trabalham com informações representadas de forma discreta, principalmente por meio do sistema binário.

Os computadores atuais são predominantemente digitais.

---

# Evolução dos Computadores

## 4. Dos dispositivos matemáticos aos computadores

A evolução dos computadores ocorreu de forma gradual, passando por dispositivos mecânicos, eletromecânicos e eletrônicos.

### Dispositivos mecânicos

Funcionavam com mecanismos físicos, sem depender de componentes eletrônicos.

#### Ábaco

Um dos primeiros instrumentos utilizados para contagem e realização de cálculos.

#### Régua de cálculo

Ferramenta utilizada para cálculos por aproximação, baseada em escalas e logaritmos.

#### Máquina de Pascal

Calculadora mecânica baseada em engrenagens, utilizada para realizar operações matemáticas.

### Charles Babbage e Ada Byron King

Charles Babbage idealizou a **Máquina Analítica**, uma máquina de propósito geral que poderia ser programada para realizar diferentes tarefas.

Ada Byron King trabalhou com Babbage e ficou conhecida por seus estudos relacionados à programação e ao uso de sequências de instruções e laços de repetição.

Resumo:

- **Babbage:** máquina programável;
- **Ada:** programação e loops.

### Dispositivos eletromecânicos

Passaram a combinar mecanismos físicos com eletricidade.

Entre os exemplos estudados estão máquinas tabuladoras, cartões perfurados e equipamentos que aumentaram o nível de automação dos cálculos.

### Dispositivos eletrônicos

A utilização de componentes eletrônicos permitiu aumentar muito a velocidade de processamento e reduzir gradualmente o tamanho das máquinas.

---

## 5. ENIAC

O ENIAC foi um importante marco da computação eletrônica.

Era uma máquina muito grande e rápida para sua época. Não possuía a flexibilidade dos computadores modernos e precisava de configurações manuais, envolvendo fios, chaves e outros componentes, para executar diferentes tarefas.

A evolução posterior permitiu que os computadores se tornassem:

- Menores;
- Mais rápidos;
- Mais eficientes;
- Mais confiáveis;
- Mais acessíveis;
- Capazes de armazenar e processar quantidades cada vez maiores de dados.

---

## 6. Gerações dos computadores

| Geração | Tecnologia característica |
| --- | --- |
| 1ª geração | Válvulas / tubos de vácuo |
| 2ª geração | Transistores |
| 3ª geração | Circuitos integrados |
| 4ª geração | Microprocessadores |

A terceira geração foi marcada pelo uso de **circuitos integrados**, que ajudaram a tornar os computadores menores, mais rápidos e mais confiáveis.

O Altair 8800 também aparece como um marco da popularização dos computadores compactos da quarta geração.

---

# Principais Componentes

## 7. Processador / CPU

A CPU é responsável por executar instruções e processar informações.

Uma forma simples de lembrar:

**CPU = executa e processa.**

### ULA - Unidade Lógica e Aritmética

Responsável por operações como:

- Soma;
- Subtração;
- Comparações;
- Operações lógicas.

### Unidade de Controle

Coordena o funcionamento interno da CPU e envia sinais de controle para que as operações sejam executadas na ordem correta.

### Registradores

Pequenas áreas de memória muito rápidas localizadas dentro do processador.

São utilizadas para guardar temporariamente dados, endereços e instruções durante o processamento.

---

## 8. Ciclo de funcionamento da CPU

O ciclo básico de execução de uma instrução é:

**Busca -> Decodificação -> Execução**

### Busca

O processador busca a próxima instrução na memória.

### Decodificação

A CPU identifica qual operação deve ser realizada.

### Execução

A operação é executada.

Resumo:

**Buscar -> Entender -> Executar**

---

## 9. Registradores importantes

### PC - Program Counter

Guarda o endereço da próxima instrução que deverá ser buscada.

### IR - Instruction Register

Guarda a instrução atual depois que ela foi buscada.

### MAR - Memory Address Register

Guarda o endereço da posição de memória que será acessada.

### MBR/MDR

Mantém temporariamente dados ou instruções transferidos entre a memória e o processador.

### AC - Acumulador

Registrador utilizado para armazenar resultados intermediários de operações.

### IBR

Na arquitetura IAS, pode manter temporariamente uma instrução que ainda será executada.

Resumo:

- **PC:** endereço da próxima instrução;
- **IR:** instrução atual;
- **MAR:** endereço de memória;
- **MBR/MDR:** dados que entram ou saem da memória;
- **AC:** resultados temporários.

---

## 10. Desvio condicional

Uma instrução de desvio permite alterar a sequência normal de execução de um programa.

Exemplo:

**Se uma condição for verdadeira, execute a instrução localizada em outro endereço.**

De forma simplificada:

1. O IR mantém a instrução;
2. A condição é avaliada;
3. A ULA participa do teste lógico;
4. Se a condição for satisfeita, o PC recebe um novo endereço.

---

## 11. Memória RAM

A memória RAM guarda temporariamente os dados e programas que estão sendo utilizados pelo processador.

Características:

- É rápida;
- É temporária;
- Seu conteúdo é perdido quando o computador é desligado;
- Quanto mais aplicações são utilizadas simultaneamente, maior tende a ser o consumo de RAM.

Resumo:

**RAM = dados temporários em uso.**

### Evolução das memórias

As memórias evoluíram em capacidade, velocidade e eficiência.

Exemplo:

**DDR4 é uma geração posterior à DDR2.**

### SRAM e DRAM

#### SRAM

- Muito rápida;
- Mais cara;
- Utilizada normalmente em memória cache.

#### DRAM

- Mais barata que SRAM;
- Utilizada como memória principal do computador.

Resumo:

**SRAM = rápida e cara -> cache**

**DRAM = memória principal -> RAM**

---

## 12. Armazenamento: HD e SSD

O armazenamento guarda dados de forma permanente.

### HD

Utiliza componentes mecânicos e partes móveis.

### SSD

Utiliza memória eletrônica e não possui partes móveis, apresentando normalmente maior velocidade de acesso aos dados.

Resumo:

**RAM != SSD/HD**

- RAM: armazenamento temporário;
- SSD/HD: armazenamento permanente.

Fluxo simplificado:

**SSD/HD -> RAM -> CPU**

Exemplo:

1. Um programa está salvo no SSD;
2. Ao ser aberto, os dados necessários são carregados na RAM;
3. A CPU executa suas instruções.

---

## 13. Placa-mãe

A placa-mãe permite a conexão e a comunicação entre os componentes do computador.

Nela estão conectados componentes como:

- CPU;
- Memória RAM;
- Armazenamento;
- Placas de expansão;
- Dispositivos internos.

---

## 14. Barramentos

### Barramento de dados

Transporta dados entre componentes.

### Barramento de endereço

Transporta os endereços das posições de memória ou dispositivos que serão acessados.

### Barramento de controle

Transporta sinais responsáveis por coordenar as operações do sistema.

---

# Modelo de Von Neumann

## 15. Conceito de programa armazenado

Antes de arquiteturas mais flexíveis, máquinas como o ENIAC precisavam ser reconfiguradas fisicamente para realizar diferentes tarefas.

O modelo de Von Neumann trouxe o conceito de **programa armazenado**.

Nesse modelo, as instruções de um programa podem ser armazenadas na memória e buscadas pelo processador para execução.

Isso tornou os computadores muito mais flexíveis, pois um mesmo hardware passou a executar diferentes programas.

Resumo:

**Antes: mudar a tarefa podia exigir reconfiguração física.**

**Von Neumann: diferentes programas podem ser armazenados e executados pela mesma máquina.**

---

## 16. Componentes do modelo de Von Neumann

De forma simplificada, a arquitetura é composta por:

- **Processador (CPU):** executa as instruções;
- **Memória:** guarda dados e instruções;
- **Entrada:** envia informações para o computador;
- **Saída:** apresenta os resultados;
- **Barramentos:** fazem a comunicação entre os componentes.

Exemplos de entrada:

- Teclado;
- Mouse;
- Microfone.

Exemplos de saída:

- Monitor;
- Impressora;
- Alto-falantes.

---

# Desempenho e Gargalos

## 17. O que é um gargalo?

Um gargalo acontece quando um componente limita o desempenho do restante do sistema.

Exemplo:

- CPU com baixa utilização;
- RAM constantemente acima de 90%;
- Sistema apresentando lentidão.

Nesse cenário, a memória RAM é o principal gargalo.

Resumo:

**Gargalo = componente que limita o desempenho geral.**

---

## 18. Backup e uso de memória

Backup é uma cópia de segurança dos dados.

Exemplo estudado:

**Backup inicia -> uso de RAM aumenta -> sistema fica lento -> CPU continua com baixa utilização.**

Nesse caso, trocar o processador não resolveria o problema.

Possíveis soluções:

- Otimizar o processo de backup;
- Realizar o backup em horários de menor uso;
- Utilizar backup incremental;
- Monitorar o consumo de recursos;
- Aumentar a memória RAM caso ela continue insuficiente.

---

## 19. Processadores multicore

Um processador multicore possui mais de um núcleo de processamento.

Exemplos:

- Single-core: 1 núcleo;
- Dual-core: 2 núcleos;
- Quad-core: 4 núcleos.

Quando uma aplicação consegue dividir perfeitamente o trabalho entre os núcleos, um processador quad-core pode, teoricamente, alcançar até quatro vezes o desempenho de um single-core equivalente.

Na prática, o ganho pode ser menor.

Resumo:

**Multicore = vários núcleos -> possibilidade de processamento paralelo.**

---

# Níveis Hierárquicos de um Sistema Computacional

## 20. Nível físico

Relacionado ao hardware.

Exemplos:

- Processador;
- RAM;
- HD/SSD;
- Barramentos;
- Clock;
- Conexões internas.

---

## 21. Nível lógico

Relacionado ao software que controla e gerencia o hardware.

Exemplos:

- Sistema operacional;
- Drivers;
- Linguagem de máquina;
- Configurações do sistema.

---

## 22. Nível de aplicação

Relacionado aos programas utilizados pelo usuário.

Exemplos:

- Simuladores;
- Editores;
- Aplicativos;
- Dados utilizados pelos programas.

Fluxo simplificado:

**Usuário -> Aplicação -> Nível lógico -> Hardware**

A ideia principal é que um problema de desempenho pode surgir em diferentes camadas.

---

## 23. Outros níveis abordados

### Nível do usuário

Aplicativos e elementos com os quais o usuário interage diretamente.

### Linguagem de alto nível

Linguagens como C e Python.

### Linguagem de montagem

Assembly é uma linguagem de baixo nível, próxima do hardware.

### Nível de controle

Coordena operações internas da CPU.

### Nível de unidades funcionais

Envolve registradores, barramentos e unidades de processamento.

### Nível das portas lógicas

Relacionado aos circuitos lógicos do computador.

---

# Revisão rápida

| Conceito | Definição curta |
| --- | --- |
| CPU | Executa instruções e processa informações |
| ULA | Realiza operações lógicas e aritméticas |
| Unidade de Controle | Coordena as operações da CPU |
| RAM | Armazena temporariamente dados em uso |
| SSD/HD | Armazenam dados de forma permanente |
| PC | Guarda o endereço da próxima instrução |
| IR | Guarda a instrução atual |
| MAR | Guarda o endereço de memória |
| MBR/MDR | Guarda temporariamente dados transferidos |
| Barramento de dados | Transporta dados |
| Barramento de endereço | Transporta endereços |
| Barramento de controle | Transporta sinais de controle |
| Gargalo | Componente que limita o desempenho |
| Backup | Cópia de segurança dos dados |
| Multicore | Processador com vários núcleos |
| Von Neumann | Arquitetura baseada em programa armazenado |

---

## Relações importantes

### Funcionamento básico

**Armazenamento -> RAM -> CPU**

### Ciclo da CPU

**Busca -> Decodificação -> Execução**

### Desvio condicional

**Condição avaliada -> se verdadeira -> PC recebe novo endereço**

### Diagnóstico de desempenho

**RAM muito alta + CPU baixa -> investigar memória**

**CPU muito alta -> investigar processamento**

**Disco sobrecarregado -> investigar armazenamento/E/S**
---

## Aula

Vídeo da aula: [Aula 01 - YouTube](https://www.youtube.com/live/a-U2oBq876Q)
