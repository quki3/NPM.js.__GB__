# MONGOOSE.__GB__
# instalacion 
```bash
npm install mongoose
```
# importar
```bash
const mongoose = require('mongoose');
```
# conectando a mongodb
## si usa una sola base de datos
```bash
  await mongoose.connect('mongodb://localhost/my_database', {
    useNewUrlParser: true,
    useUnifiedTopology: true,
    useFindAndModify: false,
    useCreateIndex: true
  });
```
## si nesecitas crear adicionales conecciones
```bash
mongoose.createConnection.
```
