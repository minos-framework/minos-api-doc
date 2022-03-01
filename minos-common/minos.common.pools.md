# minos.common.pools module


### _class_ minos.common.pools.MinosPool(\*args, maxsize=10, recycle=300, already_setup=True, \*\*kwargs)
Bases: [`minos.common.setup.MinosSetup`](minos.common.setup.md#minos.common.setup.MinosSetup), `aiomisc.pool.PoolBase`, `Generic`[`minos.common.pools.P`], `abc.ABC`

Base class for Pool implementations in minos


#### \__init__(\*args, maxsize=10, recycle=300, already_setup=True, \*\*kwargs)

#### acquire(\*args, \*\*kwargs)
Acquire a new instance wrapped on an asynchronous context manager.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`P`)



* **Returns**

    An asynchronous context manager.



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



#### _async_ close(timeout=None)

* **Return type**

    `None`



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[[`minos.common.configuration.config.MinosConfig`](minos.common.configuration.config.md#minos.common.configuration.config.MinosConfig), `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= [`minos.common.setup.MinosSetup`](minos.common.setup.md#minos.common.setup.MinosSetup))



* **Returns**

    A instance of the called class.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
