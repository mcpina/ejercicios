var http = require('http');
var contador=0;
function peticionServidor(req,resp)
{
        contador = contador + 1;        
        console.log('Contador : '+contador);
	console.log('Peticion enviada');
	resp.writeHead(200, {'Content-Type': 'text/html'});
	resp.write('<head><style type="text/css"><!--body{background-color: #33F;color: #FFF;}--></style></head><body><h1>Ejercicio 2 Modulo node.js</h1><tr><td>El Numero de  Visitas a esta WEB es:    </td><td>'+contador +'</td></tr></table></body>');
 	resp.end();
}

var s = http.createServer(peticionServidor);
s.listen(8000,'127.0.0.2');
console.log('Servidor Creado');
console.log('Servidor accediendo a http://127.0.0.2:8000/');
