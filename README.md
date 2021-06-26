# Modelagem da Interação Genótipo x Ambiente

**Curta Duração, Conceitos Básicos + tools em R, 4h**

**Idioma: Português**


Repositório dedicado ao curso GxE ministrado para o grupo EuGeM da Universidade Federal de Goiás (UFG) em 26 de junho de 2021

<img align="center" src="/fig/Curso_capa.png" width="100%" height="100%">

# Introdução

A interação GxE é um fenômeno universal entre os seres vivos. É decorrente
da interação multifatorial e não aditiva entre genótipos (conjunto de genes)
e o meio no qual se encontra (conjunto de fatores ambientais) (Lynch and Walsh,
1998). Assim, pode ser interpretada biometricamente como a diferença entre
os valores fenotípicos (conjunto de respostas observadas), ambientais e
genotípicos. A interação GxE constitui um fenômeno estatístico e biológico
de grande importância no processo de melhoramento genético de plantas,
pois desde os primeiros estágios de seleção até a estimação do valor de cultivo e uso
(VCU), para fins de recomendação de cultivares, a interação GxE dificulta a interpretação
do fenótipo observado e subsequentes inferências sobre o valor
genético (Duarte and Vencovsky, 1999). Com o advento das ômicas, sobretudo o triangulo básico do melhoramento baseado em predição (genômica, fenômica, envirômica, Crossa et al., 2021), novos modos de modelar e compreender a GxE também sugiram. Com isso, as plataformas de predição (sobretudo predição genômica) tem buscado acomodar dados de tipagem ambiental em larga escala (enviromica), além de outras ômicas e informações adicionais. Isto tem se dado tanto para explorar biologicaente a interção GxE (e.g., regressão fatorial) como para fins de predição de diversos cenários multi-ambientais, além da otimização de ensaios multi-ambientais (Rincent et al., 2017; 2019; Costa-Neto et al preprint)

# Objetivos

 - 1. Fornecer conceitos teóricos básicos para compreender o fenômeno da interação GxE a partir do trinagulo do melhoramento moderno;
 - 2. Mostrar a diferença dos modelos exploratórios empíricos e analíticos, no que tange a compreensão e predição da GxE em diversos estágios de programas de melhoramento de plantas;
 - 3. Disponibilizar códigos em programação open-source visando a democratização do uso de modelos envolvendo dados genômicos e ambientais

# Parte Teórica (1:30h)
   * Why R?
   * Dados Multi-Ambientais
   * Norma de reação via índice empírico e FW
   * GGE biplot
   * Regressão Fatorial com dados ambientais
   * Regressões Genômicas]
   * Hands-on 1: Envirotyping usando R EnvRtype
   * Hands-on 2: Predição Genômica com Envirômica
   * Questões Orientadas

A apresentação completa está disponível [aqui](https://raw.githubusercontent.com/gcostaneto/Mini_Curso_GxE_pt/main/Germano_Costa_Neto_Modeling%20GxE%20using%20phenotypic%2C%20genomic%20and%20enviromic.pdf)

# Parte Prática (no R, 2h)

Os códigos da aula prática podem ser encontrados [aqui](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/Curso_GxE.rar)

Sugestão: não rode o arquivo .rmd, trabalhe no codigo .R

- Questões-Alvo (Práticas)
- Dados Multi-Ambientais
- Norma de Reação via Regressão Linear
- GGE biplot usando Site-Regression Model
- Modelos Marca x Ambiente
- Envirotyping (Tipagem de ambientes) usando o pacote R EnvRtype
- Predições usando dados genomicos e ambientais

**Pacotes base**

- Copie e cole no R o código abaixo:

```
# funcao para instalar automatico #
call.packages <- function(pkg){
  
  new.pkg <- pkg[!(pkg %in% installed.packages()[, "Package"])]
  
  if (length(new.pkg)) for(i in 1:length(new.pkg)) install.packages(new.pkg[i], dependencies = TRUE)
    sapply(pkg, require, character.only = TRUE)
}

# vetor de pacotes (no CRAN)
pacotes_necessarios <- c('ggplot2','tidyverse','plyr','reshape2,'raster','FactoMineR','emmeans,'foreach','doParallel','gge','GGEBiplots','superheat','BGLR','plsdepot')

# instalação automático (e chamada via require)
call.packages(pkg = pacotes_necessarios) 
```

**Principais pacotes utilizados**

- **EnvRtype**: Envirotyping Tools in R ([Download](https://github.com/allogamous/EnvRtype), [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/EnvRtype.pdf))
- **BGLR**: Bayesian Generalized Linear Regression ([Download](https://github.com/gdlc/BGLR-R) , [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/BGLR.pdf))
- **BGGE**: Bayesian Genotype plus Genotype by Environment Interaction ([Download](https://github.com/italo-granato/BGGE) , [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/BGGE.pdf))
- **FW**:Bayesian method and ordinary least square method for Finlay-Wilkinson Regression. ([Download](https://github.com/lian0090/FW) , [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/FW.pdf))
- **gge** & **GGEBiplots** ([Download gge](https://kwstat.github.io/gge/) & [Download GGEBiplots](https://cran.r-project.org/web/packages/GGEBiplots/index.html), [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/tree/main/literatura/Material%20GGE))
- **metan** A R package for multi-environment analysis ([Download](https://tiagoolivoto.github.io/metan/reference/metan-package.html), [Publicação](https://github.com/gcostaneto/Mini_Curso_GxE_pt/blob/main/literatura/metan.pdf),[vinheta metan](https://cran.r-project.org/web/packages/metan/vignettes/metan_start.html))
