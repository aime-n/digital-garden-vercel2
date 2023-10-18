---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/kolmogorov-smirnov/"}
---


# Kolmogorov-Smirnov Test Procedure

>[!info] Definition
>The Kolmogorov-Smirnov (K-S) test is utilized for continuous data to test the goodness of fit, determining whether a sample follows a specific distribution.

## **Procedure Steps:**

### **1) Formulate the Hypotheses**
   - **Null Hypothesis ( $H_0$ ):** The sample follows distribution X.
   - **Alternative Hypothesis ( $H_1$ ):** The sample does not follow distribution X.

### **2) Order Data and Construct a Table**
   - Order the data in ascending order.
   - Calculate the Empirical Cumulative Distribution Function (ECDF) and the theoretical CDF.
#### ECDF

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/calculo-da-distribuicao-acumulada-empirica-ecdf/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




A Distribuição Acumulada Empírica (ECDF, sigla em inglês para Empirical Cumulative Distribution Function) é uma função estatística que **descreve a distribuição cumulativa** dos dados em um conjunto de amostras. Ela é usada para representar graficamente como os dados estão distribuídos em relação a uma variável aleatória e é uma maneira empírica de estimar a função de distribuição acumulada de uma população a partir de dados amostrais.

A ECDF é construída da seguinte maneira:

1. Ordene os dados em ordem crescente.

2. Para cada valor de dados na amostra, calcule a proporção de valores iguais ou menores a ele na amostra. Isso é feito dividindo o número de valores menores ou iguais ao valor atual pelo tamanho total da amostra.

3. Crie um gráfico de dispersão onde o eixo x representa os valores dos dados e o eixo y representa as proporções calculadas no passo 2.

A ECDF é uma representação acumulativa da distribuição dos dados e é útil para visualizar como os dados estão distribuídos em relação a uma variável aleatória. Ela permite que você identifique rapidamente características importantes da distribuição, como a mediana, os quartis e a forma geral da distribuição.

A ECDF é uma ferramenta valiosa na análise exploratória de dados, especialmente quando você deseja entender a distribuição de seus dados sem fazer suposições específicas sobre a forma da distribuição subjacente. É frequentemente usada em estatística descritiva e em gráficos de probabilidade, como o gráfico de probabilidade normal, que é usado para verificar se os dados seguem uma distribuição normal.

</div></div>

   
   **Columns of the Table:**
   - $x$: Value, ordered from smallest to largest.
   - **Order:** From 1 to the sample size.
   - $Fn(x)$: Order/n (ECDF).
   - $F0(x)$: Theoretical CDF, calculate the integral of the probability density function (pdf).
   - $|F0(x) - Fn(x)|$: $D_n$.
   - $|F0(x) - Fn(x-)|$: Crossed $D_n$.  --> subtrai o Fn da linha anterior



### **3) Find the Maximum Deviation, $d$, Value**
   - Look for $d$, i.e., the maximum value of the last two columns.

### **4) Comparison with Critical Values**
   - Compare the calculated $d$ value with the critical values given in the K-S test table, and identify the $p-value$ range.
   - If the $p-value > 0.05$, we do not reject the null hypothesis $H_0$.

   **Example for Uniform Distribution PDF:**
   - $PDF$: $(x+1)/2$

