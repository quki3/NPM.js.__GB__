# Express 

#instalacion
```bash
$ npm install express --save // --save deprecado para node.js
```
# requerimos expres
```bash
 const express = require('express')
```
# esto nos devuelve una funcion que pondremos en una constante
```bash
const app = express()
```
# esta funcion nos devuelve propiedades y methodos
```bash
  app.use //? monta una espesifica funcion o middleware en un espesifico path(ruta) esta
              middlewarefunction es ejecutada cuando la base de la peticion (requested)
              del path(ruta) coinsida con el path
              |argumentos que recibe|
              (path,callback)
                             .path => puede ser => .una string representando el path(ruta)
                                                   .A path pattern.
                                                   .una exprecion regular pattern que haga match con el path(ruta)
                                                   .un array de combinaciones de cualquiera de las anteriores
                             .callback => puede ser => una funcion middleware
     .
```
