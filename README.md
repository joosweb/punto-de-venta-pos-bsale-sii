# Bienvenidos a POS-OSAN!

OsanPOS es un sistema de control de inventario + punto venta, con una interfaz amigable
y dinamica, es una web SPA, lo cual una vez cargada no hay constantes cargas de pagina si no mas bien parece una APP, con esto los tiempos de carga son muy superiores a otros lenguajes web, si no prueba la demo publicada mas abajo en este post.

Por el momento esta habilitada la empresa [BSALE](https://www.bsale.cl/sheet/api-factura-electronica), se espera proximamente sincronizar la facturacion con LIBREDTE, ya que sabemos es un proyecto el cual utiliza una api para emitir documentos y que existe una version comunidad la cual puede instalar cualquier persona y utilizar su antes mencionada API.


## Lenguajes de programacion

El sistema esta desarrollado con estas distintas tecnologias

 1. Mysql
 2. Laravel
 3. Html
 4. Vue.JS (vue-router, vuex)
 5. $Jquery muy poco (Se pretende precindir de el pronto).

## Notificaciones

El sistema puede configurarse por SKU o CODIGO de producto.

El sistema enviará notificaciones locales, via email o ambas según se quiera, avisando con el numero de dias configurado en dicho SKU critico. Esto me permite saber con los dias que yo quiera cuando mi stock se acabara, conviertiendo una herramienta que trabaja en base a tus ventas ya sea:

 - Ultimos 4 dias
 - Ultimas 4 semanas
 - Ultimos 4 Meses

 El sistema tomara una media de venta diaria pudiendo anticipar con los dias que usted quiera el deficit de stock, para asi solicitar al proveedor con anticipacion el producto requerido.

Alertas por EMAIL

![email](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2000.30.56.png?raw=true)

Vista en el telefono

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/phone.jpg?raw=true)

## PUNTO DE VENTA

El sistema posee un punto de venta retail multiuso, donde se podran scanner con pistola de codigo de barras, ya que a su vez permite el ingreso de categorias e items para su futura venta en este POS retail,
esto logra poder procesar y genera boleta, factura, cotizacion de una manera muy simple.

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2000.24.03.png?raw=true)

> METAS POR CUMPLIR

 1. Sistema de gastos (Proximamente)
 2. Sistema de caja, manejara caja incial, cierre de caja, reportes de venta. (Proximamente).

## Sistema de reportes

El sistema permite tener un control total de tu negocio pudiendo generar reportes tales como:

 1. Total de ventas del dia, por metodo de pago, por monto, etc.
 2. Gráficos donde podras ver la curva de ventas y otros reportes.
 3. Items mas y menos vendidos.
 4. Clientes que mas y menos han comprado.
 5. Reportes de ventas donde podras ver la boleta o factura con todos sus detalles, ademas de su PDF para su posible impresión o vista.

 ![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/screencapture-192-168-1-192-8000-2020-05-16-00_22_18.png?raw=true)

## Empresas de facturacion

Actualmente esta configurada para trabajar con BSALE, pudiendo usar el plan más basico y teniendo su propio programa conectado a el para emitir documentos tributarios.

Ventajas de usar este sistema y no pagar un poco mas con BSALE mismo.

 - Puede estar instalado en tu pc teniendo los datos en tu mano y toda la infraestructura, lo que permite ademas añadir a futuro fácilmente funcionalidades extras personalizadas para tu empresa.
 -
 - No te amarra a bsale, podemos y puedes implementar infinitos sistemas de facturacion ya que si un dia encuentras otra empresa mas barata de facturacion te cambias y mantienes el mismo sistema conectado via API  a dicha empresa, bsale es el principio pero vienen mas empresas a futuro como ya habiamos mencionado mas atras posiblemente  [LibreDTE](https://libredte.cl/), un proyecto open source para la facturacion gratuita para chile, con la cual vinculado a este sistema podras emitir documentos tributarios conectados por API igualmente, con todo esto posees un completo sistema para manejar tu empresa desde la contabilidad hasta el cliente, y si eres programador el campo crece.

## Documentos tributarios

Puedes imprimir tanto en hoja de carta o papel continuo, ya que es configurable desde el panel de administracion.

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/documentos%20tributarios/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2003.29.52.png?raw=true)

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/documentos%20tributarios/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2003.31.04.png?raw=true)

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/documentos%20tributarios/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2003.31.09.png?raw=true)

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/documentos%20tributarios/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2003.31.48.png?raw=true)

# Imprime tus codigos

Los sku o codigos que insertes en el sistema pueden ser generados por el mismo o leer un producto directamente con sus codigo de barras.
Esto permite poder imprimir estos códigos por si perdiera su etiqueda o si simplemente no la tiene.

El tipo de codigo codigo usado es el CODE-129

![enter image description here](https://github.com/joosweb/punto-de-venta-pos-bsale-libredte/blob/master/screenshots/Captura%20de%20Pantalla%202020-05-16%20a%20la%28s%29%2000.26.50.png?raw=true)

Revisa la demo aqui: [POS-OSAN](http://pos.osan.cl/)

usuario: demo@osan.cl
contraseña: demo

Los datos de la demo se eliminan perdiodicamente por lo cual lo que haga en ella no quedará almecenado por mucho tiempo, es solo una muestra del sistema.
