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
  express.Router/? crea una nueva ruta objeto
                  ------------------------------
                  const { Router } = require('express');
                  const router = Router();
                  router.get('/',(req,res)=>{
                                     res.json({"Title":"hello world"})
                  })
                  module.exports = router;
  app.listen //?
     
     .get //?
     
     .post //? 
     
     .delete//?
     
     .use //? monta una espesifica funcion o middleware en un espesifico path(ruta) esta
              middlewarefunction es ejecutada cuando la base de la peticion (requested)
              del path(ruta) coinsida con el path
              |argumentos que recibe|
              (path,callback)
                             .path => puede ser => .una string representando el path(ruta)
                                                   .A path pattern.
                                                   .una exprecion regular pattern que haga match con el path(ruta)
                                                   .un array de combinaciones de cualquiera de las anteriores
                             .callback => puede ser => una funcion middleware
     .use(express.urlencoded({extended:false}))//? analiza el request retorna un middleware con un body que haga mach con type option
                                               //? type option
                                               extended : false //? permite analizar solo datos en cadena
                                               inflate :
                                               limit :
                                               parameterLimit :
                                               type :
                                               veryfi :
     .set//? asigna el nombre de configuracion a un valor podemos optener ese valor en cualquier parte de nuestra api
             --------------------------------------------------------------------------------------------------------
             app.set('port',3000)
             app.listen(app.get('port'),()=>{console.log(`server on port ${app.get('port')}`)})
```
