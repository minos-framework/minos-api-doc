# minos.common.injectors module


### _class_ minos.common.injectors.DependencyInjector(config, \*\*kwargs)
Bases: `object`

Async wrapper of `dependency_injector.containers.Container`.


#### \__init__(config, \*\*kwargs)

#### container()
Get the dependencies container.


* **Returns**

    A `Container` instance.



#### injections()
Get the injections dictionary.


* **Returns**

    A dict of injections..



#### _async_ unwire()
Disconnect the configuration.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ wire(\*args, \*\*kwargs)
Connect the configuration.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
