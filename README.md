# Pagination Bootstrap Symfony integrated.

![Version](https://img.shields.io/badge/version-1.0-green.svg)

Very simple pagination used in Symfony project with Bootstrap theme.

# How to Use

1. Add **pagination.html.twig** in your src file for example *(AcmeBundle/Resources/views)*.
2. Include a **pagination.html.twig** in your file where you want add a pagination.

we use the tag *include* of *twig*:
 ````php
{% include 'AcmeBundle/Resources/views/pagination.html.twig' with {'pagination' : pagination_array}  %}
 ````
 
with array *'pagination_array'* that contains:

* pagination_array**.page**: the number of current page (you can get it from arguments of route).
* pagination_array**.pages**: the number of pages.

**NB:** You can calculate the number of pages using php function:

 ````php
$pages = floor($total_items / $item_per_page);
 ````
