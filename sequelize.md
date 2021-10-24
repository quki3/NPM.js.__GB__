# sequelize
Promise- based Node.js ORM for Postgres, MySQL, MariaDB, SQLite and Microsoft sql Server
# instalacion
```bash
npm install --save sequelize
```
# driver de database
```bash
npm install --save pg pg-hstore
```
# conectandonos a una base de datos
```javascript
//requerimos sequelize
const Sequelize = require('sequelize');

// Option 1: Passing parameters separately
const sequelize = new Sequelize('nombredelabasededatos', 'username', 'password', {// 
  host: 'localhost',
  dialect: /* one of 'mysql' | 'mariadb' | 'postgres' | 'mssql' */
});

// Option 2: Passing a connection URI
const sequelize = new Sequelize('postgres://user:pass@example.com:5432/dbname');

```
schama
```javascript
const nombredelschema = sequelize.define('nombredelschema',{
                                    id:{
                                        type:Sequelize.INTEGER,
                                        primaryKey:true
                                    },
                                    name:{
                                        type:Sequelize.TEXT
                                    },
                                    priority:{
                                        type:Sequelize.INTEGER
                                    },
                                    description:{
                                        type:Sequelize.TEXT
                                    },
                                    deliverydate:{
                                        type:Sequelize.DATE
                                    }
                                    })
                                    
       nombredelschema.create({
                                name,
                                priority,
                                description,
                                deliverydate
                              })//crea un nuevo schema 
```
