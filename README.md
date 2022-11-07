# Sentiment Analysis

Este proyecto realiza un análisis de sentimiento expresado en el último tweet de una cuenta de twitter usando la API
de twitter y el modelo de análisis Roberta previamente entrenado

## Prerrequisitos

Vamos a necesitar algunas librerías antes de poder ejecutar el proyecto y debes tener una cuenta Developer en twitter para poder utilizar la api

Los comandos para instalar las librerías (yo use pip, tu puedes utilizar el que quieras) son los siguientes:

- pip install transformers
- pip install scipy
- pip install torch
- pip install tweepy

Ahora para poder utilizar la API debes crearte una cuenta developer en la siguiente [página](https://developer.twitter.com/en/docs/twitter-api)
Debes dar un nombre a tu proyecto, y llenar los datos que te piden. Dar permisos de read and write al proyecto

![image](https://user-images.githubusercontent.com/45043430/200388648-31f83b5b-da7e-4dc8-97da-f97c7edd5303.png)

Además asegurate de guardar bien los tokens, API secrets, client IDS, todos los secretos que se generen ya que los necesitaras para el archivo config.ini

### Resultado

Al ejecutar el comando ***.\tw-sentiment.py*** en la terminal, el programa procede a anlizar el último tweet  de tu feed de alguien que sigues e imprime algo así

![image](https://user-images.githubusercontent.com/45043430/200389809-0308a9fe-e338-4063-9099-093c31915914.png)

Denota cual fue la emoción que más predominó en ese tweet (la de mayor porcentaje, en este caso neutral). Funciona con tweets tanto en inglés como en español, también entiende emojis.
