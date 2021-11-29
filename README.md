# proyectoLogistiqal.github.io

# Proyecto Logistiqal<br>
<br>
Aplicación que permite ver la lista de productos que tienen en stock mediante una tabla. Además, la aplicación cumpla con los siguientes requisitos: <br>
● Tiene un paginador. <br>
● Se puede elegir la cantidad de registros por página. <br>
● Se puede filtrar el contenido de la tabla por el nombre del producto (Buscar). ● Tiene un diseño agradable. <br>
● Puede almacenar la siguiente información de los productos: Código único, nombre único, precio y stock. <br>
● Puede agregar, quitar y modificar los productos. <br>
<br>
Para esto usa JSP y sistema gerenciador de banco de dados (SGBD) relacional para desplegar los datos de MySql.<br>
Utiliza Bootstrap para definir el layout de las vistas y estilizar. Solicita el nombre de usuario y contraseña y un mecanismo de cierre de sesión.<br>
Contiene un CRUD para la entidad Producto, extendiendo CrudRepository. <br>
<br>
Dependencias que venían<br>
spring-boot-starter-data-jpa<br>
spring-boot-starter-web<br>
tomcat-embed-jasper<br>
javax.servlet<br>
webjars-locator<br>
bootstrap<br>
jquery<br>
<br>
Dependencias agregadas<br>
spring-boot-devtools<br>
mysql-connector-jav<br>
lombok<br>
spring-boot-starter-tomcat<br>
spring-boot-starter-test<br>
<br>
<br>
### Pre-requisitos 📋
Proyecto generado bajo <br>
Eclipse IDE for Enterprise Java and Web Developers (includes Incubating components)<br>
Version: 2021-09 (4.21.0)<br>
En Framework Spring Boot 2.5.6<br>

Tomcat v9.0<br>
<br>
Base de Datos MySQL<br>
Base de Datos = "logistiqal";<br>
Driver = "com.mysql.jdbc.Driver";<br>
Url = "jdbc:mysql://localhost/logistiqal";<br>
<br>
Con 2 tablas:<br>
CREATE TABLE `producto` (<br>
  `id_producto` int NOT NULL AUTO_INCREMENT,<br>
  `codigo` varchar(255) DEFAULT NULL,<br>
  `nombre` varchar(255) DEFAULT NULL,<br>
  `precio` varchar(255) DEFAULT NULL,<br>
  `stock` int DEFAULT NULL,<br>
  PRIMARY KEY (`id_producto`)<br>
) <br>
<br>
CREATE TABLE `usuario` (<br>
  `ID_USUARIO` int NOT NULL AUTO_INCREMENT,<br>
  `NOMBRE` varchar(200) DEFAULT NULL,<br>
  `CLAVE` varchar(200) DEFAULT NULL,<br>
  `RUT` int DEFAULT NULL,<br>
  `DV` char(1) DEFAULT NULL,<br>
  PRIMARY KEY (`ID_USUARIO`)<br>
) <br>
<br>
La única ruta planteada desde web.xml es <br>   <welcome-file>login.jsp</welcome-file><br>
<br>
Se despliegan los métodos del controlador:<br>
/login.jsp<br>
/home.jsp<br>
/error.jsp<br>
/editar.jsp<br>
/agregar.jsp<br>
<br>
<br>
## Comenzando 🚀  <br>

*Tras generar las conexiones respectivas con las tablas en AdministracionConexion.java<br>
Run As -> Spring Boot App<br>
-> Botón Derecho en Boot Dashboard y click en Open Web Browser, generando el 1er despliegue del proyecto.<br>
<br>
Podrá Ingresar en Login, Agregar productos, Editarlos, Eliminarlos, Paginarlos o Buscarlos segun muestra .Gif<br>
<br>
<br>
#### Login<br>
![1  login](https://user-images.githubusercontent.com/88750836/143794188-de92ca09-c03f-4575-a18d-a23e2b83d19f.gif)<br>
#### Agregando<br>
![2  agregando](https://user-images.githubusercontent.com/88750836/143794214-4960c13d-5a87-4d05-8688-76a41296dfff.gif)<br>
# Editando<br>
![3  editando](https://user-images.githubusercontent.com/88750836/143794241-4063a06f-557a-41c5-bfa7-fe2aaf5dedfa.gif)<br>
#### Eliminando<br>
![4  eliminando](https://user-images.githubusercontent.com/88750836/143794427-c61d8ccb-12b7-420b-8895-bf06231e11c7.gif)<br>
<br>
<br>
### Autor(es) ✒️

* **Rodolfo Stazzi S** - *Back & Front* - [<ro.sta>](https://github.com/RodStazzi)

---
