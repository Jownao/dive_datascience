# Métricas e matriz de confusão

## Exemplo de uma matriz de confusão 

* Esse modelo é de um caso de predição de transações frauduentas

<img width="420" alt="Capturar" src="https://github.com/Jownao/dive_datascience/assets/50759662/74541742-eac1-47d2-a61e-f5cee63f19fd" align = "center">

* Elemento na posição (0,0): representa a quantidade de classificações Verdadeiros Negativos, ou seja, a quantidade de vezes que o modelo acertou a predição negativa conforme os dados reais. No exemplo, o classificador previu corretamente 25377 casos em que o resultado foi de transações não fraudulentas.
* Elemento na posição (0,1): representa a quantidade de classificações Falsos Positivos, ou seja, a quantidade de vezes que o modelo previu incorretamente um resultado como positivo. No exemplo, o classificador previu, incorretamente, 4 casos em que o resultado foi fraude, sendo que a predição correta deveria ser de não fraude.
* Elemento na posição (1,0): representa a quantidade de classificações Falsos Negativos, ou seja, a quantidade de vezes que o modelo previu incorretamente um resultado como negativo. No exemplo, o classificador previu incorretamente 22 casos em que o resultado foi de não fraude, sendo que a predição correta deveria ser fraude.
* Elemento na posição (1,1): representa a quantidade de classificações Verdadeiros Positivos, ou seja, a quantidade de vezes que o modelo acertou a predição positiva conforme os dados reais. No exemplo, o classificador previu corretamente 1 caso em que houve fraude.


## Métricas
### Acurácia/Accuracy: avalia a proporção de acertos em relação a todas as previsões realizadas. É obtida somando a diagonal principal da matriz e dividindo pela soma de todos os valores.

![imagem4](https://github.com/Jownao/dive_datascience/assets/50759662/a009a4d4-1d2c-4a9c-af7d-8bbac382dd18)

* Para o exemplo dado seria:

![imagem5](https://github.com/Jownao/dive_datascience/assets/50759662/0455c4cb-49d4-4d06-8ac9-cc4c0e766cc5)

-----
### Sensibilidade/Revocação/Recall: avalia a proporção de verdadeiros positivos dentre todos os valores positivos reais. É obtida dividindo os verdadeiros positivos pela soma de positivos reais.

![imagem6](https://github.com/Jownao/dive_datascience/assets/50759662/d222ff62-0d47-4f38-bf80-900176b547a2)

* Para o exemplo dado seria:

![imagem7](https://github.com/Jownao/dive_datascience/assets/50759662/9c32e708-ec83-4876-9200-ac82d9d06da6)

-----
### Precisão/Precision: avalia a proporção de verdadeiros positivos dentre as predições dadas como positivas pelo modelo. É obtida dividindo os verdadeiros positivos pela soma das previsões positivas.

![imagem8](https://github.com/Jownao/dive_datascience/assets/50759662/913d5aec-ca33-4971-9006-1cb35b36d732)

* Para o exemplo dado seria:

![imagem9](https://github.com/Jownao/dive_datascience/assets/50759662/20a702f4-6890-4bf7-a109-2065c3e335f1)

-----
### F1 Score: é o equilíbrio entre a sensibilidade e a precisão, sendo a média harmônica entre as duas métricas.

![imagem10](https://github.com/Jownao/dive_datascience/assets/50759662/265588a3-b375-4629-8874-970efa110bfb)

* Para o exemplo dado seria:

![imagem11](https://github.com/Jownao/dive_datascience/assets/50759662/84547fe7-264d-449b-9a90-a3bd19a69077)


* Fonte: https://cursos.alura.com.br/course/modelos-preditivos-dados-deteccao-fraude
