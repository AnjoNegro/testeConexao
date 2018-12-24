const Sequelize = require('sequelize');
const sequelize = new Sequelize('usuarios', 'root', 'senha123', {
  host: 'localhost',
  dialect: 'mysql'
})





sequelize.authenticate().then(function(){
  console.log("Conecção realizada com sucesso!")
}).catch(function(erro){
  console.log("Falha ao se conectar ".erro)
})
