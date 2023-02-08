Tailwind Navwalker for WordPress
=========================================

Tailwind Navwalker is a custom WordPress nav walker class to fully implement the [Tailwind CSS framework](https://tailwindcss.com) navigation in a WordPress theme.

Features
--------

*   Compatible with latest version of Tailwind CSS framework
*   Easy to implement and customize
*   Supports WordPress menu items, including dropdown and active menu item
*   Supports custom menu fields and classes

Installation
------------

To use Tailwind Navwalker in your WordPress theme, follow these steps:

1.  Download the latest version of the class from this repository.
2.  Save the file in your WordPress theme directory, usually `wp-content/themes/your-theme/`
3.  Include the class in your theme's `functions.php` file by adding the following line:

phpCopy code

`require_once get_template_directory() . '/tailwind-navwalker.php';`

Usage
-----

To display the menu in your theme, you can use the following code in your template file:

phpCopy code

`<?php   wp_nav_menu( array(     'theme_location'  => 'primary',     'container'       => false,     'menu_class'      => '',     'fallback_cb'     => '',     'menu_id'         => 'main-menu',     'walker'          => new Tailwind_Navwalker(),   ) );   ?>`

Customization
-------------

You can customize the output of the menu by modifying the `$args` array passed to the `wp_nav_menu` function.

For example, to add additional classes to the menu's container, you can modify the `menu_class` argument:

phpCopy code

  `'menu_class'      => 'tailwind-navbar-menu',`

You can also add custom classes to individual menu items by using the WordPress menu item's `classes` field.

Conclusion
----------

Tailwind Navwalker makes it easy to implement Tailwind CSS navigation in your WordPress theme. With its easy customization options, you can quickly create a navigation that fits your theme's style.