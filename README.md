# Modelagem da Interação Genótipo x Ambiente

**Curta Duração, Básico, 4h**

**Idioma: Português**


Repositório dedicado ao curso GxE ministrado para o grupo EuGeM da Universidade Federal de Goiás (UFG) em 26 de junho de 2021

<img align="center" src="/fig/Curso_capa.png" width="100%" height="100%">

# Introdução

A interação GxE é um fenômeno universal entre os seres vivos. É decorrente
da interação multifatorial e não aditiva entre genótipos (conjunto de genes)
e o meio no qual se encontra (conjunto de fatores ambientais) (Lynch and Walsh,
1998). Assim, pode ser interpretada biometricamente como a diferença entre
os valores fenotípicos (conjunto de respostas observadas), ambientais e
genotípicos. Por esse motivo, constitui um fenômeno estatístico e biológico
de grande importância no processo de melhoramento genético de plantas,
pois desde os primeiros estágios de seleção até a estimação do valor de cultivo e uso
(VCU), para fins de recomendação de cultivares, a interação GxE dificulta a interpretação
do fenótipo observado e subsequentes inferências sobre o valor
genético (Duarte and Vencovsky, 1999). Com o advento das ômicas, sobretudo o triangulo básico do melhoramento baseado em predição (genômica, fenômica, envirômica, Crossa et al., 2021), novos modos de modelar e compreender a GxE também sugiram. Com isso, as plataformas de predição (sobretudo predição genômica) tem cada vez mais se adaptado para acomodar dados de tipagem ambiental em larga escala (enviromica) para fins de predição de diversos cenários multi-ambientais. 

# Objetivos

 - 1. Fornecer conceitos teóricos básicos para compreender o fenômeno da interação GxE;
 - 2. Mostrar a diferença dos modelos exploratórios empíricos e analíticos, no que tange a compreensão e predição da GxE em diversos estágios de programas de melhoramento de plantas;
 - 3. Disponibilizar códigos em programação open-source visando a democratização do uso de modelos envolvendo dados genômicos e ambientais

# Parte Teórica
- Questões-Alvo (Teoricas)
- Causas da Variação Fenotípica
- Decomposição da Variação Fenotípica
- Histórico da G×E ao longo dos últimos  60 anos
- Ambiente e sua Tipologia
- Norma de Reação e Plasticidade Fenotípica
- Adaptabilidade e Estabilidade
- Predição de Fenótipos sob múltiplas condições ambientais
- Covariâncias Genomicas e Enviromicas

A apresentação completa está disponível [aqui]()

# Parte Prática (no R)

**Principais pacotes utilizados**

- **EnvRtype**: Envirotyping Tools in R ([Download](https://github.com/allogamous/EnvRtype), [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/EnvRtype.pdf))
- **BGLR**: Bayesian Generalized Linear Regression ([Download](https://github.com/gdlc/BGLR-R) , [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/BGLR.pdf))
- **BGGE**: Bayesian Genotype plus Genotype by Environment Interaction ([Download](https://github.com/italo-granato/BGGE) , [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/BGGE.pdf))
- **FW**:Bayesian method and ordinary least square method for Finlay-Wilkinson Regression. ([Download](https://github.com/lian0090/FW) , [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/FW.pdf))
- **gge** & **GGEBiplots** ([Download gge]() & [Download GGEBiplots](), [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/jkab040.pdf))
- **metan** A R package for multi-environment analysis ([Download](https://tiagoolivoto.github.io/metan/reference/metan-package.html), [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/metan.pdf),[vinheta metan](https://cran.r-project.org/web/packages/metan/vignettes/metan_start.html))

# Bibliografia Recomendada

* [Modelagem Fenótipo sob multiplos ambientes](#P1)
* [Tipagem de ambientes em larga escala (large-scale envirotyping, in short, enviromics)](#P6)
* [Modelagem Fenótipo-Ambiente (Phenotype-Envirotype, dados ambientais)](#P2)
* [Modelagem Genótipo-Fenótipo (Genotype-to-Phenotype)](#P3)
* [Modelagem Norma de Reação Genômica (linear regressions)](#P4)
* [Modelagem Norma de Reação Genômica (kernel methods)](#P5)

----------------------------------------------------------------------------------------------------

<div id="P1" />

**Modelagem Fenótipo sob múltiplos ambientes (caracterizar GxE histórica)**


<div id="P2" />

**Modelagem Fenótipo-Ambiente (Phenotype-Envirotype, dados ambientais)**


<div id="P6" />

**Tipagem de ambientes em larga escala (large-scale envirotyping, in short, enviromics)**

<div id="P3" />

**Modelagem Genótipo-Fenótipo (Genotype-to-Phenotype)**



<div id="P4" />

**Modelagem Norma de Reação Genômica (linear regressions)**


<div id="P5" />

**Modelagem Norma de Reação Genômica (kernel methods)**

