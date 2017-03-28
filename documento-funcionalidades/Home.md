![https://www.utec.edu.pe/sites/default/files/logo_0.png](http://www.utec.edu.pe/sites/default/files/logo_utec_.png)

# Funcionalidades del Modulo de {NOMBRE MODULO}

En este documento se encuentran todas las funcionalidades complejas de este modulo.

## Tramites de Retiro de asignatura
1. El alumno solicita el retiro de un curso matriculado a través de la pantalla de solicitud de trámite.
2. El sistema valida los parametros de la configuracion de trámite de retiro de asignatura.
3. La solicitud se registra satisfactoriamente.
4. El jefe de secretaría académica ingresa a la pantalla de Consulta de solicitudes
5. El jefe ingresa al detalle de la solicitud y la aprueba.
6. El sistema actualiza el estado Aprobado en la tabla ACA_SOLICITUD_TRAMITE y el estado Retirado en ACA_ALUMNO_MATRICULA_CURSO.

## Tramites de Retiro de Ciclo
1. El jefe de secretaria académica ingresa a la pantalla de consulta de solicitudes de trámites y selecciona el tipo de solicitud a registrar.
2. El jefe busca el alumno y se cargan los campos de la pantalla.
3. El jefe guarda la solicitud y se validan los parámetros de la configuración del trámite para el último periodo de matricula del alumno.
4. El jefe busca la solicitud guardada en la pantalla de busqueda de solicitudes.
5. El jefe aprueba la solicitud
6. El sistema actualiza el estado Aprobado en la tabla ACA_SOLICITUD_TRAMITE y el estado Retirado en ACA_ALUMNO_MATRICULA asi como para todos los cursos en los que se encuentre matriculado ACA_ALUMNO_MATRICULA_CURSO.

## Tramites de Retiro de Universidad
1. El jefe de secretaria académica ingresa a la pantalla de consulta de solicitudes de trámites y selecciona el tipo de solicitud a registrar.
2. El jefe busca al alumno y se cargan los campos de la pantalla.
3. El jefe guarda la solicitud y se validan los parámetros de la configuración del trámite para la ultima matricula del alumno.
4. El jefe busca la solicitud guardada en la pantalla de búsqueda de solicitudes.
5. El jefe aprueba la solicitud
6. El sistema actualiza el estado Aprobado de la solicitud en la tabla ACA_SOLICITUD_TRAMITE y se actualiza el username del alumno a .old, además de actualizar el estado de su malla actual a Inactivo. Si el alumno tiene una matricula en el periodo actual, se realiza el retiro de ciclo.

## Tramites de Reingreso
1. El jefe de secretaria académica ingresa a la pantalla de consulta de solicitudes de trámites y selecciona el tipo de solicitud a registrar.
2. El jefe busca al alumno y se cargan los campos de la pantalla.
3. El jefe selecciona el periodo en el que el alumno va a reingresar.
3. El jefe guarda la solicitud y se validan los parámetros de la configuración del trámite para el periodo seleccionado.
4. El jefe busca la solicitud guardada en la pantalla de búsqueda de solicitudes.
5. El jefe aprueba la solicitud
6. El sistema actualiza el estado Aprobado de la solicitud en la tabla ACA_SOLICITUD_TRAMITE

# Colaboradores
*  Lizbeth Mamani Salce
