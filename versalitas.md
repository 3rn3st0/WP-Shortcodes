#Shortcode Versalitas

Shortcode para Wordpress que permite agregar texto en formato [versalitas](http://es.wikipedia.org/wiki/Versalita) de manera sencilla.

Las instrucciones siguientes deben ser agregadas en el archivo `functions.php` de nuestro theme o en archivos propios que serían llamados desde `functions.php`.
```PHP
// Función de llamada (callback function)
function shrtcod_versalitas($atts, $content = null) {
	return '<h3 class="versalitas">' . $content . '</h3>';
}

// Registro del shorcode dentro de nuestro Theme
add_shortcode('versalitas', 'shrtcod_versalitas');
```


Las instrucciones siguientes deben ser agregadas en el archivo `style.css` de nuestro theme.
```CSS
/* Texto en formato versalitas */
.versalitas { font-variant: small-caps; }
```
