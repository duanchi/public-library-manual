## Class \Net\Http\Client\Request

> Provide a Http Request.

### How to Use

```php
$__request   =   new \Net\Http\Client\Request(EX_NET_HTTP_METHOD_GET, 'http://localhost');

$__request
    ->set('Dump', mktime())
    ->set('File', \Core\UUID::make());

```


### Methods
----

> \Net\Http\Client::__construct

> \Net\Http\Client->set

> \Net\Http\Client->get

> \Net\Http\Client->execute


### Properties
----

> \Net\Http\Client->url

> \Net\Http\Client->method

> \Net\Http\Client->http_version

> \Net\Http\Client->request_body

> \Net\Http\Client->request_header

> \Net\Http\Client->ssl_options

> \Net\Http\Client->*


### Constants
----

> EX_NET_HTTP_METHOD_GET

> EX_NET_HTTP_METHOD_DELETE

> EX_NET_HTTP_METHOD_HEAD

> EX_NET_HTTP_METHOD_TRACE

> EX_NET_HTTP_METHOD_OPTIONS

> EX_NET_HTTP_METHOD_POST

> EX_NET_HTTP_METHOD_PUT

> EX_NET_HTTP_METHOD_PATCH

> EX_NET_HTTP_METHOD_UPDATE




### \Net\Http\Client::__construct
----

Init a \Net\Http\Client\Request instance with `new \Net\Http\Client\Request();`


#### Define

```php
public void \Net\Http\Client::__construct (
    string $_method = '',
    string $_url = '',
    string $_request_body = '',
    array $_request_headers = [],
    array $_ssl_options = []
)
```

#### Parameters


##### _method

> type :　`string`

> desc : Http request method.

> value : EX\_NET\_HTTP\_METHOD\_*



##### _url

> type :　`string`

> desc : Http request url.



##### _request_body

> type :　`string`

> desc : Http request body or form.



##### _request_header

> type :　`array`

> desc : Http request headers.

> value : ['Key', 'Value'] or [['Key1', 'Value1'], ['Key2', 'Value2']...]



##### _ssl_options

> type :　`array`

> desc : Ssl options.

> value : ['Key', 'Value'] or [['Key1', 'Value1'], ['Key2', 'Value2']...]





### \Net\Http\Client->set
----

Set a property, header or property/header list to current request.


#### Define

```php
public Client \Net\Http\Client::set (string $_key = '', mixed $_value = '')

public Client \Net\Http\Client::set (array $_list)
```

#### Parameters

##### _key

> type :　`string`

> desc : Key of property,header.



##### _value

> type :　`mixed`

> desc : value of property,header.



##### _list

> type :　`array`

> desc : Couple or list of property,header.

> value : ['Key', 'Value'] or [['Key1', 'Value1'], ['Key2', 'Value2']...]

