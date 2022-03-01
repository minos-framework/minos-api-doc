# minos.networks.discovery.clients.memory module


### _class_ minos.networks.discovery.clients.memory.InMemoryDiscoveryClient(\*args, \*\*kwargs)
Bases: [`minos.networks.discovery.clients.abc.DiscoveryClient`](minos.networks.discovery.clients.abc.md#minos.networks.discovery.clients.abc.DiscoveryClient)

In Memory Discovery Client class.


#### \__init__(\*args, \*\*kwargs)

#### _property_ is_subscribed(_: boo_ )
Check if the client is subscribed or not.


* **Return type**

    `bool`



* **Returns**

    


#### _property_ route(_: st_ )
Get the full http route to the discovery.


* **Return type**

    `str`



* **Returns**

    An `str` value.



#### _async_ subscribe(\*args, \*\*kwargs)
Subscribe to the discovery.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ unsubscribe(\*args, \*\*kwargs)
Unsubscribe from the discovery.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
