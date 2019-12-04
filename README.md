# Transbank Opencart 3.x Webpay Plugin

## Descripción

Este plugin de Opencart 3.x implementa 
el [SDK PHP de Transbank](https://github.com/TransbankDevelopers/transbank-sdk-php) 

## Dependencias

* transbank/transbank-sdk (composer)
* fpdf


## Instalación del plugin para un comercio

El manual de instalación para el usuario final se encuentra disponible [acá](docs/INSTALLATION.md) o 
en PDF [acá](https://github.com/TransbankDevelopers/transbank-plugin-opencart-webpay/blob/master/docs/INSTALLATION.pdf)


## Nota  
- La versión del sdk de php se encuentra en el archivo `config.sh` y 
en `src/upload/system/library/transbank/composer.json`

**NOTA:** La versión del sdk de php se encuentra en el script config.sh

## Preparar el proyecto para bajar dependencias

    ./config.sh

## Crear una versión del plugin empaquetado 

    ./package.sh

## Desarrollo

Para apoyar el levantamiento rápido de un ambiente de desarrollo, hemos creado la especificación de contenedores a 
través de Docker Compose.

Para usarlo seguir el siguiente [README Opencart 3.x](./docker-opencart3)

### Actualizar el PDF de instalación
Instalar `markdown-pdf` con `npm i -g markdown-pdf` y luego para generar el archivo `INSTALLATION.pdf` sea debe ejecutar: 
```
cd docs/
markdown-pdf INSTALLATION.md
```
