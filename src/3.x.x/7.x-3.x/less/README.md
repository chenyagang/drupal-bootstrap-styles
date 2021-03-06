# [Drupal Bootstrap Styles] (LESS)

These files are intended to be used within a [Drupal Bootstrap] based sub-theme.

## Default Variables

The `variable-overrides.scss` file is generally where you will spend the
majority of your time providing any default variables that should be
used by the [Bootstrap Framework] instead of its own.

> **WARNING:** It is highly recommended that you only put the default variables
  you intend to override in this file. Copying and pasting the entire
  `variables.less` file provided by the [Bootstrap Framework] is redundant and
  only makes it more difficult to determine which variable has been overridden
  when the need to update or upgrade to newer versions in the future arises. 

## Drupal Bootstrap

The `drupal-bootstrap.less` file contains various styles to properly integrate
[Drupal Bootstrap] with the [Bootstrap Framework].

## Compiling

The `style.less` file is the main compiling entry point. It is the glue that
combines: `variable-overrides.less`, [Bootstrap Framework Source Files] and the 
`drupal-bootstrap.less` files together. Generally, you will not need to modify
this file unless you need to add or remove files to be imported.

Your [Less] compiler should use this file as it's "source" and its compiled
output "destination" should be `../css/style.css` (overwrites the file provided
by the base-theme starterkit).

[Bootstrap Framework]: https://getbootstrap.com/docs/3.4/
[Bootstrap Framework Source Files]: https://github.com/twbs/bootstrap-sass
[Drupal Bootstrap]: https://www.drupal.org/project/bootstrap
[Drupal Bootstrap Styles]: https://github.com/unicorn-fail/drupal-bootstrap-styles
[Less]: http://lesscss.org
