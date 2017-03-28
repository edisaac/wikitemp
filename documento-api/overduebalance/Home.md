![https://www.utec.edu.pe/sites/default/files/logo_0.png](http://www.utec.edu.pe/sites/default/files/logo_utec_.png)

# Deuda Atrasada

----
  Retorna la deuda atrasada relacioanda al codigo de alumno ingresado.

## API

 `http://host:port/comercial-api/v2`  
  
## URL

 `alumno/cuenta/overdue`

## Metodo

  `Get`
  
## Cabeceras de la Petición

Nombre		  | Tipo	         	| Valor
------------- | ------------------- | -------------
Content-Type  | string 				| application/json
X-Auth-Token  | string 				| ---
  
## Parámetros URL

Nombre		  | Tipo	         	| Requerido
------------- | ------------------- | -------------
codigoAlumno  | string 				| si

## Parámetros BODY

  `None`

## Respuesta Exitosa

```json
{
  "timestamp": 1484922433086,
  "status": 200,
  "error": null,
  "message": "OK",
  "managed": true,
  "content": {
    "overduebalance": "336.00"
  }
}
```
 
## Error Response

```json
{
  "timestamp": null,
  "status": 200,
  "error": null,
  "managed": false
  "message": null,
}
```

## Error Codes

Status		  | Mensaje	         	                        | Descripcion
------------- | ------------------------------------------- | -------------
201			  | Sistema externo no responde 				| Mas detalle 




