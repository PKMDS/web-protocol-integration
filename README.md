# Web protocol integration

Maneja la integracion de las aplicaciones que se invocan por el protocolo web `filingCabinet:`. 

A continuacion la descripcion de cada proyecto:

## handler

Maneja los parametros enviados por el protocolo web que invocaran una aplicacion. El formato de los parametros es el siguiente:

```json
filingCabinet:{
  app: string, // indica al aplicacion a abrir. ejemplo: fc scan, fc admin, fc web. etc, etc.
  parameters:{ }// objeto dinamico que le sera enviado a la aplicacion como parametro
}
```

## ProtocolRegister

Registra el protocolo en los registros de windows registry.
