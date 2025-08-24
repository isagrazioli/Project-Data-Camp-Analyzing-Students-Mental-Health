# Project-Analyzing-Students-Mental-Health

## Sobre o Projeto: 
Uma universidade internacional japonesa pesquisou seus alunos em 2018 e publicou um estudo no ano seguinte que foi aprovado por vários conselhos éticos e regulatórios. O estudo descobriu que os estudantes internacionais têm um risco maior de dificuldades de saúde mental do que a população em geral, e que a conexão social (pertencimento a um grupo social) e o estresse aculturativo (estresse associado à adesão a uma nova cultura) são preditivos da depressão.

## Objetivo análise: 
Validar essa conclusão e investigar se a duração da estadia é um fator que contribui para a depressão entre esses estudantes. Processo: agrupando todos os estudantes internacionais por tempo de estadia. Para cada grupo (cada ano de estadia), calculo:
count_int: O número total de estudantes.
average_phq: A média de sintomas de depressão (provavelmente do questionário PHQ-9).
average_scs: A média da pontuação de conexão social.
average_as: A média da pontuação de estresse de aculturação.

## Ferramentas:
Notebook, SQL.

## Principais descobertas: 
1) Estresse de Aculturação Aumenta com o Tempo: Há uma tendência relativamente clara de que o estresse associado à adaptação a uma nova cultura (average_as) aumenta com o tempo de estadia, especialmente nos primeiros 4 anos. A média sobe de 72.8 no primeiro ano para 87.71 no quarto ano.
2) Sintomas de Depressão Também Mostram Aumento Inicial: A média de sintomas de depressão (average_phq) também parece ter uma tendência de alta nos primeiros anos, indo de 7.48 (ano 1) para um pico de 9.09 (ano 3).
3) Conexão Social Permanece Estável: A pontuação de conexão social (average_scs) não mostra uma tendência óbvia de subida ou descida nos grupos com mais estudantes, mantendo-se relativamente estável na faixa de 37-38.

Ponto Crítico de Atenção: O Tamanho da Amostra. O número de estudantes (count_int) diminui drasticamente para estadias mais longas. Tenho uma boa quantidade de dados para estadias de 1 a 4 anos (95, 39, 46, 14 estudantes, respectivamente). As conclusões para esses grupos são mais confiáveis.
Para estadias de 5 anos ou mais, o número de estudantes é muito baixo (1, 3, 2, 1, 1). As médias calculadas para esses grupos não são estatisticamente relevantes e podem ser enganosas, pois são baseadas em pouquíssimas pessoas. Por exemplo, a altíssima média de depressão (average_phq de 13) para 10 anos de estadia representa a opinião de apenas um estudante.

Conclusão Resumida: Para estudantes internacionais, os primeiros anos de estadia são marcados por um aumento no estresse de aculturação e nos sintomas de depressão, enquanto o sentimento de conexão social não se altera significativamente. A hipótese original do estudo parece se confirmar, e sim, a duração da estadia parece ser um fator contribuinte, especialmente nos primeiros anos.
