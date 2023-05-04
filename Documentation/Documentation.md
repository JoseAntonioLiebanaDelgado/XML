# XML

<?xml version=“1.0” encoding=“UTF-8”?>


## Caracteres Especiales 
<br>
- &lt : <
- &gt : >
- &amp : &
- &apos : '
- &quot : "
<br>

## CDATA

- Al utilizar la sección CDATA, el contenido entre las etiquetas se trata simplemente como una cadena de caracteres sin procesar y no se realizan interpretaciones o traducciones especiales.
  
- Por ejemplo, si se quisiera incluir la siguiente frase en un documento XML: "El símbolo ' < ' es utilizado para abrir etiquetas en XML", se podría escribir como:
<texto><![CDATA[El símbolo ' < ' es utilizado para abrir etiquetas en XML]]></texto>
<br>

## Feed
- Un feed o canal es un archivo generado por el sitio web, que contiene una versión específica de la información publicada en esa web.
<br>

## RSS

<rss version=“2.0”>
    <channel>
        ... Contenido ...
    </channel>
</rss>

- RSS es un formato de archivo XML que permite a los sitios web publicar actualizaciones de contenido en tiempo real. Es un formato abierto y libre bajo licencia de Creative Commons.

- <title>: es el nombre del canal, la forma con la que se conoce el servicio
  
-<description>: descripción corta del contenido del canal

-<link>: enlace a la dirección donde esta el contenido HTML que se quiere mostrar con el canal o feed


<rss version="2.0">
    <channel>
        <title>W3Schools Home Page</title>
        <link>http://www.w3schools.com</link>
        <description>Free web building tutorials</description>
        <item>
            <title>RSS Tutorial</title>
            <link>http://www.w3schools.com/rss</link>
            <description>New RSS tutorial on W3Schools</description>
            <category>News</category>
            <category>Tutorial</category>
            <pubDate>Fri, 28 Apr 2010</pubDate>
        </item>
    </channel>
</rss>


## Etiqueta <pubDate>
La representación de las fechas en RSS sigue la especificación RFC 822, y ha de seguir la estructura siguiente:
Dia de la semana, Dia Mes Año Hora:Minuto:Segundos Zona horaria
Dia de la semana: “Mon”, “Tue”, “Wed”, “Thu”, “Fri”, “Sat”, “Sun”.
Mes: “Jan”, “Feb”, “Mar”, “Apr”, “May”, “Jun”, “Jul”, “Aug”, “Sep”, “Oct”, “Nov”, “Dec”
Año: siempre ha de tener 4 dígitos.


# XSD
- Restricciones en valores:
- El elemento ”age” no puede tener un valor menor que 0 ni mayor que 120.
- El elemento ”car” se restringe a los valores Audi, Golf y BMW.
- El elemento ”letter” admite una letra minúscula entre la a y la z.
- El elemento ”password” se restringe  a una longitud igual a 8 caracteres.

### Order indicators:
• All
• Choice
• Sequence
### Occurrence indicators:
• maxOccurs
• minOccurs