# minos.networks.utils module


### _class_ minos.networks.utils.Builder(\*args, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`, `abc.ABC`, `Generic`[`minos.networks.utils.Instance`]

Builder class.


#### \__init__(\*args, \*\*kwargs)

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



#### _abstract_ build()
Build the instance.


* **Return type**

    `typing.TypeVar`(`Instance`)



* **Returns**

    A `BrokerSubscriber` instance.



#### copy()
Get a copy of the instance.


* **Return type**

    `typing.TypeVar`(`B`, bound= `minos.networks.utils.Builder`)



* **Returns**

    A `BrokerSubscriberBuilder` instance.



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



#### _classmethod_ new()
Get a new instance.


* **Return type**

    `typing.TypeVar`(`B`, bound= `minos.networks.utils.Builder`)



* **Returns**

    A `BrokerSubscriberBuilder` instance.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### with_config(config)
Set config.


* **Parameters**

    **config** (`minos.common.configuration.config.MinosConfig`) – The config to be set.



* **Return type**

    `typing.TypeVar`(`B`, bound= `minos.networks.utils.Builder`)



* **Returns**

    This method return the builder instance.



#### with_kwargs(kwargs)
Set kwargs.


* **Parameters**

    **kwargs** (`dict`[`str`, `typing.Any`]) – The kwargs to be set.



* **Return type**

    `typing.TypeVar`(`B`, bound= `minos.networks.utils.Builder`)



* **Returns**

    This method return the builder instance.



### _async_ minos.networks.utils.consume_queue(queue, max_count)
Consume `count` at least `1` and at most `max_count` elements from the given queue.


* **Parameters**

    
    * **queue** – The queue to be consumed.


    * **max_count** (`int`) – The max count of elements to be consumed.



* **Return type**

    `None`



* **Returns**

    This function does not return anything.



### minos.networks.utils.get_host_ip()
Get the host ip.


* **Return type**

    `str`



* **Returns**

    A string value.



### minos.networks.utils.get_host_name()
Get the host name.


* **Return type**

    `str`



* **Returns**

    A string value.



### minos.networks.utils.get_ip(name)
Get the ip address.


* **Parameters**

    **name** (`str`) – The name to be converted to an ip.



* **Return type**

    `str`



* **Returns**

    A string value.
