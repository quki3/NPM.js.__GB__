# MORGAN.__GB__
registra las solicitudes del http.
Es un logeador de request cada ves que alla un request morgan nos puede indicar informacion en la consola de este req.

# como usarlo 
# instalacion
```bash
npm i morgan
```
# inport
```bash
import express from 'express'
```
# es un middleware por tanto podemos usarlo de express
```bash

app.use(morgan('tiny'))//?GET / 404 139 - 8.014 ms
app.use(morgan("short'))//?::1 - GET / HTTP/1.1 404 139 - 7.649 ms
app.use(morgan('combined'))//?::1 - - [10/Jul/2021:19:55:11 +0000] "GET / HTTP/1.1" 404 139 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36 Edg/91.0.864.64"
app.use(morgan('common'))//?::1 - - [10/Jul/2021:19:53:03 +0000] "GET / HTTP/1.1" 404 139
app.use(morgan('dev'))//? GET / 404 7.236 ms - 139
```
