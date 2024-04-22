# Clase Docker

IMPORTANTE:
Este ejemplo asume que el dataset de MNIST está ubicado en `../MNIST`
Descargar train.csv y test.csv de MNIST [acá](https://www.kaggle.com/c/digit-recognizer/data)

## Build

```bash
sudo docker build -t mnist-udesa .
```

## Run

```bash
sudo docker run --publish 8231:8231 -v $PWD/../MNIST/:/MNIST/ -v $PWD:/solution/ mnist-udesa
```
