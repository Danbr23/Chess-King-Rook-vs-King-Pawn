# Projeto de Data-Science e Machine-Learning com Base de Dados de Xadrez

Curso: Engenharia de Computação - IFSULDEMINAS - Campus Poços de Caldas<br>
Matéria: Inteligência Artificial<br>
Professor: Douglas Castilho Braz

Projeto de Data Science e Machine Learning com base de dados de jogos de xadrez para prever se as brancas vão vencer ou não.

## Visão Geral do Conjunto de Dados

 O dataset **KRKPA7** descreve posições de fim de jogo de xadrez envolvendo **rei e torre (brancas) contra
 rei e peão em a7 (pretas)**. São ao todo **3196 posições** distintas registradas, cada uma avaliada quanto
 à possibilidade de vitória das brancas. As posições são representadas por **36 atributos categóricos** que
 codificam características da configuração no tabuleiro, seguidos de 1 atributo alvo indicando o
 resultado (vitória ou não das brancas). Não há atributos numéricos; todos os 36 atributos são
 categóricos com valores simbólicos (como f , t, n, g, etc.). Não existem valores ausentes no
 conjunto – todos os 36 atributos estão preenchidos para cada instância . Cada atributo geralmente
 1indica se determinada condição posicional ou tática é verdadeira (t de true) ou falsa (f de false)
 naquela posição, embora alguns atributos usem outros códigos categóricos específicos (como n , g, 
l , w, b) para indicar estados particulares (discutidos adiante). 

O conjunto de dados possui duas classes-alvo: **"won"** (brancas podem forçar a vitória) e **"nowin"**
 (brancas não conseguem forçar vitória). Das 3196 posições, **1669 (cerca de 52%)** são posições em que as
 brancas podem vencer, e **1527 (48%)** são posições em que as brancas não conseguem vitória (ou seja,
 as pretas conseguem pelo menos um empate ou vencer) . Portanto, as classes estão relativamente
 balanceadas (ligeiro predominância de posições vencedoras para as brancas). Cada instância é
 representada como uma sequência de 36 valores categóricos seguida pelo rótulo "won" ou "nowin"
 indicando se White-can-win (brancas vencem) ou White-cannot-win 

# Roteiro:

## Pré-processamento e Análise

1. Identificação do atributo alvo (saída);
2. Identificação dos tipos de dados dos atributos de entrada (quantitativo, qualitativo);
3. Identificação da escala de dados dos atributos de entrada (nominal, ordinal, intervalar,
racional);
4. Exploração dos dados através de medidas de localidade;
5. Exploração dos dados através de medidas de espalhamento;
6. Exploração dos dados através de medidas de distribuição;
7. Identificação e separação do conjunto de teste, que será utilizado para testar o desempenho
dos modelos – o conjunto de testes deve ser representativo e ter as características da
população completa. Caso sua base de dados já tenha o conjunto de teste definido, analisar
se este segue as características do conjunto de treinamento;
8. Identificação e eliminação de atributos não necessários;
9. Identificação e eliminação de exemplos não necessários;
10. Análise e aplicação de técnicas de amostragem de dados (caso não seja necessário, analisar
o porquê);
11. Identificação e aplicação de técnicas para minimizar problemas de desbalanceamento (caso
não seja necessário, analisar o porquê);
12. Limpeza de dados:<br>
  a. Identificação e eliminação de ruídos ou outliers;<br>
  b. Identificação e eliminação de dados inconsistentes;<br>
  c. Identificação e eliminação de dados redundantes;<br>
  d. Identificação e resolução de dados incompletos (ausentes) – utilização de alguma
técnica de preenchimento e justificar;

13. Identificação e conversão dos tipos de dados (caso não seja necessário, analisar o porquê).
Os tipos de conversão que podem ser utilizados são:
a. Conversão de tipos (simbólico para numérico, ordinal para numérico, nominal para
binário, numérico para ordinal);
b. Normalização dos dados (re-escala ou padronização);
14. Análise e aplicação de alguma técnica para redução de dimensionalidade – pesquisar
alguma técnica utilizada na literatura e aplicar;

## Análise Preditiva

1. Definição da técnica de validação a ser utilizada (cross-validation, hold-out, leave-one-out,
etc);
2. Definição das métricas a serem utilizadas para avaliar os resultados preditivos dos modelos
(acurácia, precisão, recall, matriz de confusão, etc);
3. Definição de um algoritmo base (baseline), que será utilizado como base para análise dos
resultados – algoritmo classe majoritária;
4. Criação de modelo preditivo utilizando algoritmo de indução baseado nos vizinhos mais
próximos e similaridade de dados (K-NN);
5. Criação de modelo preditivo utilizando algoritmo de indução baseado em árvores de
decisão (decision tree ou árvore C4.5);
6. Criação de modelo preditivo utilizando algoritmo de indução redes neurais artificiais
(MLP);
7. Análise dos resultados do algoritmo baseline;
8. Análise dos resultados dos três algoritmos de aprendizado de máquina supracitados;

## Resultados

