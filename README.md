# Parcial1JS

Objetivo de el parcial:
Se debe desarrolalr una API REST utilizando Express  que permita administrar 
solicitudes de soporte tecnico dentro de una empresa.

La empresa TechSupport S.A. necesita un sistema sencillo para registrar incidencias 
reportadas por sus empleados.

Cada incidencia representa un problema tecnico que debe ser atenndido por el departamento
de TI.

Para poder poner a prueba con algunos datos que eh pensado ya podemos poner en el new request:
Antes ejecutar en la terminal: npm run dev

Registrar una incidencia: POST http://localhost:3000/incidencias
    "{
      "empleado": "Juan Perez",
      "area": "Contabilidad",
      "descripcion": "No puedo imprimir documentos",
      "prioridad": "Alta"
    }"

Listar las incidencias registradas: GET http://localhost:3000/incidencias

Buscar incidencias por el id: GET http://localhost:3000/incidencias/1

Cambiar el estado de una incidencia ya creada: PUT http://localhost:3000/incidencias/1/estado
    "{
    "estado": "En Proceso"
    }"

Eliminar incidencias: DELETE http://localhost:3000/incidencias/ "numero a eliminar"

Estadisticas: GET http://localhost:3000/incidencias/estadisticas

Clasificar automaticamente: GET http://localhost:3000/incidencias/1/clasificacion