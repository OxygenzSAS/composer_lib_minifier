# minifier
minifier middleware

# install

```
composer require oxygenzsas/composer_lib_minifier

```

# utilisation

Exemple d'utilisation 
```js
$tableau_middleware[] = new \OxygenzSAS\Minifier\Minifier(
    ['css_folder_1','css_folder_2', ...] // list css folders
    , ['js_folder_1','js_folder_2', ...] // list js folders
    ,86400 // cache time ms
);
```

Exemple d'utilisation dans le framework oxygenzsas/app
```php
//...
$tableau_middleware[] = new \OxygenzSAS\Minifier\Minifier(
    \OxygenzSAS\Framework\Plugin::getInstance()->getAllCSSFolders()
    , \OxygenzSAS\Framework\Plugin::getInstance()->getAllJSFolders()
    ,86400
);
//...
```
