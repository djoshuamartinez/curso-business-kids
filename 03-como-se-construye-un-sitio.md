[Volver](README.md)
# ¿Cómo se construye un sitio?

Bueno, ahora si, con nuestro objetivo bien claro, comenzemos a hacer un sitio...

Pero antes de lanzarnos a ver las maneras en las que puedes plasmar tus ideas, debes preguntarnos algo importante:

## ¿Qué es un sitio web?
Un sitio web en realidad es una colección de archivos que están en una computadora que tiene acceso a la red y está configurada para compartir esos archivos. Esta computadora puede ser como cualquier otra que hayas visto, incluso la tuya. Como la computadora está en la red, para que se puedan comunicar a ella, se requiere de una dirección, que la puedes pensar como la dirección de tu casa, es decir, palabras o identificadores que te dicen como llegar a tu casa, la dirección con la que se identifica en la red, se llama *dirección IP* y todas las computadoras conectadas a la red deben tener una, otorgada por nuestro router.

Esa dirección es lo que necesitamos para entrar a la página web que esté compartiendo esa computadora. Hagamos un experimento, en una *consola de comandos*, escríbamos lo siguiente:
```
ping google.com
```
Si estás conectado a la red, verás que se comienzan a escribir cosas en pantalla, aprieta ENTER para que deje de escribir. Lo que hicimos fue mandar paquetes a la dirección web que le dijimos (que fue google.com) y ver si los paquetes estaban llegando exitosamente a esa computadora.

Claro que esa dirección `google.com` no es una dirección IP, ese es un nombre amigable, la dirección IP fue lo que nos respondió la consola: 172.217.17.78
Esa es la dirección que la computadora que comparte google en la red tiene asociada.

Para que te convenzas de eso, puedes colocar esa dirección en un *navegador de internet* que es con lo que nuestra computadora se comunica con otras computadoras a través de ciertos protocolos, ejemplos de ellos son Firefox, Chrome, Safari, Opera, Internet Explorer, entre otros. ¡Verás que sucede lo mismo que si hubieras escrito google.com! Si quieres conocer la dirección que tu computadora tiene en la red, puedes ejecutar en consola:
```
ipconfig
```
Que te da información sobre tu conexión a la red global, en específico tu dirección IP, e incluso la dirección asociada al router. Si colocas tu dirección en un navegador, fallará, pues no has configurado a tu computadora en la red para que comparta archivos que sean tu sitio web. Pero si colocas la del router, ¡verás que hay un sitio que te permite administrar el mismo router!

Bueno, pero afortunadamente, nosotros no tenemos que recordar 172.217.17.78 cada que queramos entrar a Google, basta con que nosotros escribamos google.com y listo.

Para que la red sepa hacer esto, se requieren de *Servidores de Nombre de Dominio* o *DNS* que en breve, son nombres amigables para las direcciones de las computadoras en la red. Nombres amigables permiten que tus clientes no entren a una dirección IP, y en lugar solo escriban el nombre de tu negocio.

Estos nombres amigables pueden ser locales, puedes colocar una lista de nombres y asociarles direcciones IP a los que corresponden esos nombres, pero eso solo serviría para ti (en una computadora con Windows, esta lista es un archivo que está en C:\Windows\System32\drivers\etc\hosts). Lo que sería deseable es que este nombre amigable funcionara en todas las computadoras, en especial las de tus clientes.

Para eso, se utilizan otras computadoras especiales en la red, que se encargan de mantener una lista de nombres amigables y las direcciones IP asociadas a las que todos recurren, se les llaman *Servidores DNS*. Para poner tu nombre en esas listas, normalmente debes pagar por ello, esto es la compra de dominios que puedes obtener de sitios como *GoDaddy*, *Google Domain*, entre muchos, muchos otros.

Por cierto, aunque hemos dicho que un sitio web son archivos que comparte una computadora en la red, no hemos mencionado que a esa computadora se le conoce como *servidor*.

Bueno, configurar una computadora como la tuya para que sea un servidor, es decir, que comparta una colección de archivos como un sitio web, no es tan fácil como lo que hemos hecho. Y aunque es posible, hay varias desventajas de que una computadora personal sea un servidor, como el gasto de energía que consume (un servidor debe estar siempre prendido), lo caliente que pueda estar por estar tanto tiempo prendido, entre otras cosas. Por ello hay empresas que se dedican a ofrecerte computadoras configuradas y prendidas que ellos tienen para que tu les des los archivos que quieras compartir y que sean tu página web. A estas empresas se les conoce como empresas de *hosting*.

![Racks de servidores](https://b2evolution.net/media/blogs/whb/shutterstock_105784187.jpg "Racks de servidores")

Bueno, a las empresas de hosting les tienes que dar archivos y decirles cosas sobre como compartir los archivos, esto depende mucho del tipo de sitio que tengas y tus necesidades, y muchas empresas ofrecen distintas maneras de compartir tus archivos.

Algunas empresas que se dedican a rentar servidores son: DigitalOcean, Atlantic.net, Amazon Web Services, GoDaddy, Hostgator, entre muchas otras. Varían en el grado de experiencia técnica que necesitas para configurar los servidores, la libertad que te ofrecen, y las características físicas del equipo que estés rentando.

La decisión de que hosting usar, deberá de ser consultada con alguien técnico que conozca los pros y contras de acuerdo a tus necesidades.

Como sea, al hosting le tienes que dar archivos, ¿qué tipo de archivos? ¿qué tipos de archivos conoces? ¿Podrías poner un archivo de Word en la computadora de la empresa de hosting que escogiste? Bueno, aquí se empieza a poner técnico, para que las computadoras entiendan que tus archivos son un sitio web, los archivos deben ser de cierto tipo especial, normalmente código de cierto tipo. Pero veremos más de eso después.

## Servicios para crear sitios

Como ves, hay mucha complejidad detrás de crear un simple sitio web, y apenas hemos arañado la superficie. Hay empresas que saben que son muchas cosas y no esperan que la gente sepa todo esto para tener un simple sitio web.

Estas empresas ya ni siquiera necesitan que les des los archivos, ellos los generan por ti, según lo que tu desees. Con estas empresas ya no te tienes que preocupar por hosting, pues ellos mismo te lo dan, y muchas veces tampoco del DNS (nombre de dominio). Es decir, te ofrecen el paquete completo y sin preocupaciones. ¡Excelente! que más podríamos querer. Cuando los sitios son simples y no deseas meterte en complejidad, y no te interesa ahorrarte lo poco que te podrías ahorrar haciéndolo tu mismo, este estilo de servicios son todo lo que necesitas. Servicios conocidos de este estilo, son Wix, Wordpress, Squarespace, Weebly, entre otros. Y se les conoce como *Site builders*.

Los sitios son muy amigables y tradicionalmente tienen editores *WYSIWYG* (What you see is what you get) , que son editores con controles dinámicos muy fáciles de usar

La desventaja de utilizar site builders para tu página es para empezar que el precio se eleva un poco, lo que es natural por todas las cosas que te están ahorrando. Sin embargo si deseas hacer tu mismo la página sin meterte tanto en la computadora, y tienes la inversión disponible. Esta es una muy buena opción.

Los sitios de Wix históricamente han tenido problemas de rendimiento, en tiempos de carga, que en el acelerado mundo que vivimos, pueden hacer que clientes se vayan.

Otra desventaja de usar estos servicios, es que estamos atados a usar sus soluciones, así si queremos hacer un sitio más dinámico, o que incorpore funcionalidades como tiendas en línea u otras cosas, podremos hacerlo, pero con las restricciones del site builder y claro, aumentando el precio.

**Actividad 2**. Como sea, estas herramientas son tan sencillas de usar que podemos ir a [Wix](https://wix.com) o  a [Wordpress](https://wordpress.com) y comenzar a explorar lo que nos pueden ofrecer. Estoy seguro que no causarán mucho problema, sus interfaces son tan amigables y parecidas a lo que estamos acostumbrados a usar en nuestro día a día que crear un sitio solo es cuestión de darnos el tiempo de hacerlo.
