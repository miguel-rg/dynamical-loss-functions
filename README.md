# Dynamical loss functions for Machine Learning

This repository contains the code that reproduces the main results of our paper [Tilting the playing field: Dynamical loss functions for machine learning](https://arxiv.org/abs/2102.03793).

## What is a dynamical loss function?

Loss functions are one of the pillars of supervised learning. They quantify the performance of the model at classifying the training data, and training a neural network reduces to minimizing one specific loss function. In this work we propose that changing the loss function during training (minimization) can lead to better results. In a dynamical loss function, we weight equally the contribution of each sample belonging to the same class, and then oscillate these weights during minimization. During each oscillation the model focuses more in one class, and we tipically cycle through all classes many times during training. 


## Why should I care?

In our [paper](https://arxiv.org/abs/2102.03793) we show:

* Using a dynamical loss function enables learning when the neural network is too small or the learning rate is too large for the model to learn the training data using standard cross entropy loss. 

* Using a dynamical loss function improves generalization in cases where the model was already able to learn the data when using standard loss functions.

* Dynamical loss functions lead to complex learning dynamics. The loss function landscape is changing as training progresses, the valleys that the model is descending during training are oscillating in high and width, what leads to instabilities when the valleys are too narrow. These instabilities appear as bifurcations in the learning dynamics that occur when the largest eigenvalue of the Hessian crosses a threshold.


## Running the code

You can run our code as a Colaboratory Notebook [dynamical_loss_functions_for_machine_learning](https://github.com/miguel-rg/dynamical-loss-functions/blob/main/dynamical_loss_functions_for_machine_learning.ipynb).







# Título del Proyecto

_Acá va un párrafo que describa lo que es el proyecto_

## Comenzando 🚀

_Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._

Mira **Deployment** para conocer como desplegar el proyecto.


### Pre-requisitos 📋

_Que cosas necesitas para instalar el software y como instalarlas_

```
Da un ejemplo
```

### Instalación 🔧

_Una serie de ejemplos paso a paso que te dice lo que debes ejecutar para tener un entorno de desarrollo ejecutandose_

_Dí cómo será ese paso_

```
Da un ejemplo
```

_Y repite_

```
hasta finalizar
```

_Finaliza con un ejemplo de cómo obtener datos del sistema o como usarlos para una pequeña demo_

## Ejecutando las pruebas ⚙️

_Explica como ejecutar las pruebas automatizadas para este sistema_

### Analice las pruebas end-to-end 🔩

_Explica que verifican estas pruebas y por qué_

```
Da un ejemplo
```

### Y las pruebas de estilo de codificación ⌨️

_Explica que verifican estas pruebas y por qué_

```
Da un ejemplo
```

## Despliegue 📦

_Agrega notas adicionales sobre como hacer deploy_

## Construido con 🛠️

_Menciona las herramientas que utilizaste para crear tu proyecto_

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - El framework web usado
* [Maven](https://maven.apache.org/) - Manejador de dependencias
* [ROME](https://rometools.github.io/rome/) - Usado para generar RSS

## Contribuyendo 🖇️

Por favor lee el [CONTRIBUTING.md](https://gist.github.com/villanuevand/xxxxxx) para detalles de nuestro código de conducta, y el proceso para enviarnos pull requests.

## Wiki 📖

Puedes encontrar mucho más de cómo utilizar este proyecto en nuestra [Wiki](https://github.com/tu/proyecto/wiki)

## Versionado 📌

Usamos [SemVer](http://semver.org/) para el versionado. Para todas las versiones disponibles, mira los [tags en este repositorio](https://github.com/tu/proyecto/tags).

## Autores ✒️

_Menciona a todos aquellos que ayudaron a levantar el proyecto desde sus inicios_

* **Andrés Villanueva** - *Trabajo Inicial* - [villanuevand](https://github.com/villanuevand)
* **Fulanito Detal** - *Documentación* - [fulanitodetal](#fulanito-de-tal)

También puedes mirar la lista de todos los [contribuyentes](https://github.com/your/project/contributors) quíenes han participado en este proyecto. 

## Licencia 📄

Este proyecto está bajo la Licencia (Tu Licencia) - mira el archivo [LICENSE.md](LICENSE.md) para detalles

## Expresiones de Gratitud 🎁

* Comenta a otros sobre este proyecto 📢
* Invita una cerveza 🍺 o un café ☕ a alguien del equipo. 
* Da las gracias públicamente 🤓.
* etc.
