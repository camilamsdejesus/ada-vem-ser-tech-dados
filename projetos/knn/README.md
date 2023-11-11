# 1 - Projeto K-Nearest Neighbors (KNN)

## Alunos:
- Felipe de Oliveira Franco
- Pedro Lima Pilon
- Camila de Jesus
- Janaina Sousa de Oliveira
- Anna Paula Schuenck Jandre

## Professora:
Renata Marchese

## Turma:
1104

---

## K-Nearest Neighbors - KNN

O K-Nearest Neighbors (KNN) é um modelo supervisionado de machine learning utilizado para classificação e regressão. Este algoritmo se baseia na proximidade entre os pontos de dados e é capaz de rotular ou aproximar valores.

### Algoritmo

1. **Definir um valor para K (por exemplo, K=5).**
2. **Definir os K vizinhos mais próximos do ponto a ser classificado de acordo com uma função de distância.**
3. **Se for um problema de Regressão: Calcular a média de todos os vizinhos. Se for um problema de Classificação: Calcular a moda de todos os vizinhos.**
4. **Atribuir o valor/classe ao ponto de interesse conforme cálculo do Passo 3.**

### Definição do Problema

Os dados fornecidos representam o cadastro de clientes de uma empresa de logística de entrega de alimentação. Cada cliente possui informações sobre quanto foi gasto nas últimas 4 compras e uma classificação de NPS: Promotor, Neutro, Detrator. O objetivo é estimar a classificação de NPS para novos clientes não classificados com base em suas últimas compras.

Os dados seguem o padrão:
```
[CPF: INT, Classificação NPS: STRING, Valor das últimas compras feitas pelo cliente: TUPLA]
```

### Regras
- Criar funções conforme necessidade.
- Não usar módulos externos como numpy e math.
- Utilizar apenas objetos e fluxos vistos até o momento no curso.

### Entrega
- Grupos de 4 a 5 alunos.
- Entrega até dia 27/10.
- Entrega de um notebook com a classificação de NPS desses novos clientes.
- Enviar arquivo .ipynb ou link do github através do LMS.

---

## Objetivo

Este projeto em equipe, parte do encerramento do primeiro módulo do curso, tem como finalidade desenvolver um sistema de classificação de dados baseado no algoritmo K-Nearest Neighbors (KNN). A implementação é realizada completamente do zero, sem a utilização de bibliotecas ou funções prontas.

A missão inclui a aplicação dos conteúdos vistos durante o módulo de lógica de programação 1 para o desenvolvimento de um código em Python para o funcionamento do KNN. Isso abrange desde o cálculo das distâncias até a escolha do valor de 'k', criando um sistema para classificar os dados.

Ao final do projeto, espera-se alcançar uma compreensão preliminar do KNN, suas nuances e desafios de implementação, bem como a capacidade de aplicar esse conhecimento para classificar conjuntos de dados.

---

## Metodologia

O projeto envolveu a organização e planejamento das atividades em equipe. Reuniões semanais foram realizadas para elaboração do projeto, incluindo a divisão de tarefas, definição de papéis e estabelecimento de um cronograma para garantir a conclusão dentro do prazo estabelecido.

---

## Conclusão

Para resolver o problema apresentado, foi realizada a implementação do algoritmo K-Nearest Neighbors (KNN) para classificar os clientes com base na classificação dos dados mais próximos.

Foram implementadas funções para calcular a distância entre dois pontos, classificar um cliente individual e classificar vários clientes sem classificação.

Durante os testes, observou-se que para valores de K inferiores a dez, não houve mudanças muito significativas na classificação. Dos trinta dados classificados, dez foram como 'Promotor', dez como 'Neutro' e dez como 'Detrator' usando valores para K de 1 a 9.

Pequenas variações foram observadas quando escolhíamos um número par para K, evidenciando a necessidade de considerar métodos de desempate para esses casos. Para valores de K maiores que 10, o modelo apresentou variações significativas na classificação, possivelmente devido às limitações do número de amostras para o treinamento do sistema.

Com o desenvolvimento do projeto, exercitamos os conhecimentos adquiridos durante as aulas, principalmente em relação à manipulação de listas, tuplas e funções, e utilização de estruturas de repetição.
