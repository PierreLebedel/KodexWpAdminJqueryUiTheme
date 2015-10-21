# WordPress admin jQueryUI Theme

A WordPress stylesheet for according jQuery UI elements to admin area.

This files are created with the [jQueryUI ThemeRoller](http://jqueryui.com/themeroller/).

The jquery-ui.css and jquery-ui.min.css files are including both structure and theme. The index.html file is an example page with many jQueryUI components.

Screenshots
--------------

1. Datepicker, Accordion, Tabs
![enter image description here](http://kodex.pierros.fr/wp-content/uploads/screenshot-11.png)

2. Slider, Progressbar, Buttons & Selectmenu, Icons
![enter image description here](http://kodex.pierros.fr/wp-content/uploads/screenshot-21.png)

3. Dialog
![enter image description here](http://kodex.pierros.fr/wp-content/uploads/screenshot-31.png)

Usage
-----
To include this theme in your plugin, use PHP code :

```php
add_action('admin_enqueue_scripts', 'kodex_admin_enqueue_scripts');
function kodex_admin_enqueue_scripts(){
	wp_enqueue_style('kodex_jqueryui', plugin_dir_url(__FILE__).'jqueryui/jquery-ui.min.css');
	wp_enqueue_script('kodex_plugin', plugin_dir_url(__FILE__).'script.js', array('jquery', 'jquery-ui-core', 'jquery-ui-datepicker'));
}
```
