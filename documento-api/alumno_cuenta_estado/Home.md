![https://www.utec.edu.pe/sites/default/files/logo_0.png](http://www.utec.edu.pe/sites/default/files/logo_utec_.png)

# Estado de Cuenta

----
  Retorna la deuda atrasada relacioanda al codigo de alumno ingresado.

## API

 `http://host:port/comercial-api/v2`  
  
## URL

 `alumno/cuenta/estado`

## Metodo

  `POST`
  
## Cabeceras de la Petición

Nombre		  | Tipo	         	| Valor
------------- | ------------------- | -------------
Content-Type  | string 				| application/json
X-Auth-Token  | string 				| ---
  
## Parámetros URL

Nombre		  | Tipo	         	| Requerido  			| Descripcion
------------- | ------------------- | --------------------- | ------------
email  		      | string 				| si				| Email perteneciente a la universidad
fechaVencimiento  | string 				| si				| Fecha con el formato : yyyymmdd. Ejemplo : 20161031
estadoDocumento   | string 				| si				| Valores soportados : **open**

## Parámetros BODY

```json
{
	"email": "jordy.aguilar@test.com",
	"fechaVencimiento": "",
	"estadoDocumento": "open"
}
```

## Respuesta Exitosa

```json
{
  "timestamp": 1484928488624,
  "status": 200,
  "error": null,
  "message": "OK",
  "managed": true,
  "content": [
    {
      "ID": "27764",
      "CONCEPTO": "CUOTA Nro 5 2016-2",
      "FECHA DE VENCIMIENTO": "7/12/2016",
      "MONTO SOLES": "1007.20",
      "MONTO DOLARES": "0",
      "COMPROBANTE": "BO 001-00036740",
      "FECHA DE PAGO": "",
      "ESTADO": "open",
      "DEUDA EN SOLES": "1007.2"
    },
	{
	},
	{
	},....
  ]
}
```
 
## Error Response

```json
{
  "timestamp": null,
  "status": 200,
  "error": 303,
  "managed": false
  "message": "Codigo de alumno no existe en el ERP.",
}
```

## Error Codes

Error		  | Mensaje	         	                        | Descripcion
------------- | ------------------------------------------- | -------------
303			  | Codigo de alumno no existe en el ERP.							| El email ingresado esta vinculado a un codigo de alumno que no existe en el erp
304			  | Codigo de alumno no existe en el Systema Academico o no guarda relacion con el email ingresado.		| 
305			  | ABC es un campo requerido.										| Un valor requerido no fue enviado. Ejmplo : "Email es un campo requerido".
306			  | El estado de cuenta ingresado tiene un valor no soportado.		| Solo el valor **open** es soportado