# minos.networks.discovery.connectors module


### _class_ minos.networks.discovery.connectors.DiscoveryConnector(client, name, host, port, endpoints, \*args, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`

Discovery Connector class.


#### \__init__(client, name, host, port, endpoints, \*args, \*\*kwargs)

#### _property_ already_destroyed(_: boo_ )
Already Destroy getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _property_ already_setup(_: boo_ )
Already Setup getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ subscribe()
Send a subscribe operation to the discovery.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ unsubscribe()
Send an unsubscribe operation to the discovery.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
