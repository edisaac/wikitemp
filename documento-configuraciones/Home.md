![https://www.utec.edu.pe/sites/default/files/logo_0.png](http://www.utec.edu.pe/sites/default/files/logo_utec_.png)

# Documento de Configuarciones

## Drupal settings.php

Este archivo debe contener :

* Urls de todas las apis con las que interactua. Mas detalle sobre las apis requeridas en la sección **documento de recursos requeridos**
    - seguridad api
    - ubigeo api
    - simulador-api
    - curricula api

* Códigos a enviar a apis especificas
    - **program_code** : Valor 1 por defecto. Este valor se envia al api curricula
    - **pre-period** : Valor 2017-1 por defecto. Este valor se envia al api ???
    - **pre_code** : Valor FICOPRE01 por defecto. Este valor se envia al api simulador, el cual a su vez se lo envia al api netsuite
    - **constant_credit** : Valor 1 por defecto. Este valor se envia al ???

## Oauth2

Para que las apis descritas anteriormente puedan funcionar, se requiere configuraciónes en la base de datos del core educativo.

La web al ser de acceso público, no tiene login previo, por lo que las apis deben configurarse para que puedan ser consumidas por el metodo [Cliente sin Login Interactivo (machine->api)](https://bitbucket.org/utecsup/documentacion-de-aplicaciones/wiki/apis/seguridad-api/endpoint_s2a_auth/Home)

Los registros para este tipo de autenticación se encuentran en la tabla : **seg_aplicacion_client**

## Roles & Usuarios (SUPER IMPORTANTE)

Estos son los siguientes roles usados en este proyecto:

???

# Colaboradores
*  Richard Leon (rleon@utec.edu.pe)
