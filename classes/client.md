## Class \Net\Http\Client

> Provide one or a list of Http Request(s) and Callbackable while Http Request(s) responed.

### How to Use

```php
$__request_handle   =   new \Net\Http\Client();

$__request_handle
    ->add_request(
        new \Net\Http\Client\Request(EX_NET_HTTP_METHOD_GET, 'http://localhost'),
        function() {
            echo 'Responsed!'
        }
    )
    ->add_request(...);
    ->execute();

```


### Methods
----

> \Net\Http\Client::__construct

> \Net\Http\Client->add_request

> \Net\Http\Client->execute

### Properties
----

> None


### Constants
----

> EX_NET_HTTP_CLIENT_STATUS_INIT

> EX_NET_HTTP_CLIENT_STATUS_EXEC

> EX_NET_HTTP_CLIENT_STATUS_RESPONDED

> EX_NET_HTTP_REQUEST_CONCURRENT




### \Net\Http\Client::__construct
----

Init a \Net\Http\Client instance with `new \Net\Http\Client();`


#### Define

```php
public void \Net\Http\Client::__construct (array $_configuration  = [])
```

#### Parameters


##### _configuration

> type :　`array`

> desc : configs of this Http Client instance.

> value : See [PECL-HTTP Configuration Manual](http://devel-m6w6.rhcloud.com/mdref/http/Client/Curl#Configuration:)





### \Net\Http\Client->add_request
----

Enqueue a request to current Client.


#### Define

```php
public Client \Net\Http\Client::add_request (Client\Request $_request, mixed $_callback_func = NULL)
```

#### Parameters


##### _request

> type :　`\Net\Http\Client\Request`

> desc : Http request instance.




##### _callback_func

> type :　`Mixed`

> desc : Call a user function while the request responed.

> value : Type `string` if defined a function or static method, type `Closure` if defined a anonymous or closure function.



### \Net\Http\Client->execute
----

Enqueue a request to current Client.


#### Define

```php
public Client \Net\Http\Client::add_request (Client\Request $_request, mixed $_callback_func = NULL)
```

#### Parameters


##### _request

> type :　`\Net\Http\Client\Request`

> desc : Http request instance.




##### _callback_func

> type :　`mixed`

> desc : Call a user function while the request responed.

> value : Type `string` if defined a function or static method, type `Closure` if defined a anonymous or closure function.


