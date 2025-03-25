# tech_challenge_2 - Grupo 11 - Ygor Guimarães
tech_challenge_2
Sobre o Projeto
Este repositório contém a solução para o Tech Challenge da Fase 2 do curso de Inteligência Artificial e Machine Learning. O projeto implementa um sistema de otimização para alocação de desenvolvedores em projetos de TI utilizando Algoritmos Genéticos.



O Problema
A alocação eficiente de recursos humanos em projetos de tecnologia é um desafio constante para empresas. Os gerentes de projeto precisam equilibrar diversos fatores:

Diferentes níveis de habilidade dos desenvolvedores
Múltiplas competências necessárias por projeto (Frontend, Backend, Database, etc.)
Prioridades variadas entre projetos
Restrições de tempo e disponibilidade
Este é um problema de otimização combinatória complexo, ideal para aplicação de algoritmos genéticos, onde o espaço de soluções possíveis é extremamente amplo.

Solução Implementada
Nossa abordagem utiliza Algoritmos Genéticos para encontrar a melhor alocação possível de desenvolvedores em projetos, considerando:

Maximização de projetos concluídos - com prioridade para os mais importantes
Utilização eficiente dos recursos - alocando as horas disponíveis dos desenvolvedores
Correspondência de habilidades - garantindo que desenvolvedores atendam aos requisitos mínimos
Estrutura do Projeto
O projeto é implementado em um Jupyter Notebook com as seguintes células:

Importação de bibliotecas e configuração inicial
Definição das classes Desenvolvedor e Projeto
Geração de dados de teste
Implementação da classe Indivíduo para o algoritmo genético
Operadores genéticos (seleção, cruzamento e mutação)
Implementação do algoritmo genético
Execução do algoritmo e medição de desempenho
Visualização dos resultados
Implementação de abordagem gulosa para comparação
Visualizações comparativas
Conclusões e análises finais
Como Utilizar
Pré-requisitos
Python 3.8+
Jupyter Notebook
numpy
pandas
matplotlib
seaborn
tqdm

O algoritmo genético implementado consegue eficientemente:

Completar projetos prioritários (100% dos projetos de prioridade 8-10)
Utilizar 99.9% das horas disponíveis dos desenvolvedores
Alocar desenvolvedores com níveis adequados de habilidade para cada projeto
Convergir para uma solução ótima em aproximadamente 40 gerações
As visualizações incluídas demonstram:

Evolução do fitness ao longo das gerações
Percentual de conclusão dos projetos por prioridade
Utilização dos recursos de cada desenvolvedor
Distribuição de horas por competência em cada projeto
Alocação detalhada do desenvolvedor mais utilizado
Comparação com Abordagem Gulosa
Implementamos também uma heurística gulosa para comparação:

Métrica	Algoritmo Genético	Heurística Gulosa
Tempo de execução	7.37s	0.0049s
Fitness	-218.58	76.76
Projetos completos	4/8	5/8
Embora a abordagem gulosa seja significativamente mais rápida e complete um projeto a mais, o algoritmo genético prioriza melhor os projetos por importância e otimiza a alocação de competências de forma mais estratégica.
