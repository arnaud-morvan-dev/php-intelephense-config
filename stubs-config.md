# Stubs config #

1. Create a .config folder on the local machine (example -> user/.config)

2. Create a stubs folder user/.config/stubs

3. Integrate the various stubs that are needed

    <ins>Exemple:</ins>

    - acf.php
    - gutenberg.php
    - laravel.php
    - woocommerce.php
    - wpbakery.php

4. Inside each file, place the key functions

5. Update the settings.json file on [Visual Studio Code](https://code.visualstudio.com/)
   
```
{
    "php.suggest.basic": false,

    "intelephense.stubs": ["wordpress"],

    "intelephense.environment.includePaths": [
        "~/projets/.config/intelephense/stubs"
    ],

    "intelephense.diagnostics.undefinedFunctions": false,
    "intelephense.diagnostics.undefinedConstants": false,
    "intelephense.environment.phpVersion": "8.2"
}
