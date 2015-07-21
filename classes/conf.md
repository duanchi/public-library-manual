## Class CONF

> Get config of keys in applications & this library.


### CONF::set_environment ($\_environment = 'base', $\_application = NULL)

> Set `CONF` environment first, then use `CONF::get()` `CONF:set()` `CONF::has()`

code:

```
\CONF::set_environment('devel', '1461791293');
```



### CONF::get($\_scope, $_key = '', $\_environment = NULL, $\_application = NULL)

> Get config vaules with scope,key,environment,applications

code:

```
\CONF::get('application', 'view');
```

Returns the `view` value in `1461791293_application_devel.ini`.

```
array(5) {
  ["engine"]=>
  string(5) "Blitz"
  ["path"]=>
  string(22) "APPLICATION_PATH/views"
  ["include_path"]=>
  string(30) "APPLICATION_PATH/views/include"
  ["include_suffix"]=>
  string(14) ".inc.tmpl.html"
  ["suffix"]=>
  string(10) ".tmpl.html"
}
```


### CONF::has ($\_scope, $_key = '', $\_environment = NULL, $\_application = NULL)

> Check config if or not exist with scope,key,environment,applications

code:

```
\CONF::has('application', 'view');
```

Return `true` while the key in `1461791293_application_devel.ini`, otherwise, return `false`.

```
bool(true)
```
