### DESAFIO DE PROJETO AWS SAGEMAKER CANVAS - DIO


Dentro do desafio utilizei um dataset disponibilizado pela comunidade da DIO, por ser mais didático e prático. Optei por indicar a coluna QUANTIDADE EM ESTOQUE, como alvo. O modelo criado após o StandardBuild (mais longo, em torno de 2h) recebemos as seguintes métricas:

Avg. wQL 0.569 -Perda Média Ponderada por Quantil; Como dito pelo professor, quando começa com zero, significa que a inteligência absorveu de forma positiva o treinamento.

MAPE 0.069 -Erro Percentual Absoluto Médio- Essa métrica calcula a diferença média entre os valores previstos e reais;

WAPE 0.691 -Erro Percentual Absoluto Ponderado- calcula a diferença média entre valores previstos e reais, com uma ponderação adicional. Essa ponderação considera a importância de cada ponto de dados, tornando-o mais adequado para séries temporais com grandes picos ou flutuações sazonais.

RMSE 4.141 -Raiz do Erro Quadrático Médio- Essa métrica mede a distância média entre os valores previstos e reais, elevando os erros ao quadrado antes de calcular a média. Essa elevação penaliza mais os erros maiores, tornando o RMSE útil para identificar grandes discrepâncias. ** Nota-se que aqui o número ficou elevado, o que sugere que o aprendizado não foi tão satisfatório.

MASE 0.000 -Erro Escalado Absoluto Médio- compara o erro médio absoluto do seu modelo com um modelo de referência simples, como a média das séries temporais. Essa comparação normaliza o erro e o torna independente da escala dos dados, facilitando a comparação entre diferentes séries temporais. ** obtivemos aqui um modelo muito satisfatório. Os feriados obtiveram uma avaliação de 100% de impacto no nosso estoque.


