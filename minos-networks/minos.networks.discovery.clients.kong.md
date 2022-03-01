# minos.networks.discovery.clients.kong module


### _class_ minos.networks.discovery.clients.kong.KongDiscoveryClient(host, port)
Bases: [`minos.networks.discovery.clients.abc.DiscoveryClient`](minos.networks.discovery.clients.abc.md#minos.networks.discovery.clients.abc.DiscoveryClient)


#### \__init__(host, port)

#### _property_ route(_: st_ )
Get the full http route to the discovery.


* **Return type**

    `str`



* **Returns**

    An `str` value.



#### _async_ subscribe(host, port, name, endpoints, retry_tries=3, retry_delay=5)
Perform a subscription query.


* **Parameters**

    
    * **host** (`str`) – The ip of the microservice to be subscribed.


    * **port** (`int`) – The port of the microservice to be subscribed.


    * **name** (`str`) – The name of the microservice to be subscribed.


    * **endpoints** (`list`[`dict`[`str`, `str`]]) – List of endpoints exposed by the microservice.


    * **retry_tries** (`int`) – Number of attempts before raising a failure exception.


    * **retry_delay** (`float`) – Seconds to wait between attempts.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ unsubscribe(name, retry_tries=3, retry_delay=5)
Perform an unsubscribe query.


* **Parameters**

    
    * **name** (`str`) – The name of the microservice to be unsubscribed.


    * **retry_tries** (`int`) – Number of attempts before raising a failure exception.


    * **retry_delay** (`float`) – Seconds to wait between attempts.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
