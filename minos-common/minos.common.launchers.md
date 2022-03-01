# minos.common.launchers module


### _class_ minos.common.launchers.EntrypointLauncher(config, injections, services, log_level=20, log_format='color', log_date_format=DateFormat.color, external_modules=None, external_packages=None, \*args, \*\*kwargs)
Bases: [`minos.common.setup.MinosSetup`](minos.common.setup.md#minos.common.setup.MinosSetup)

EntryPoint Launcher class.


#### \__init__(config, injections, services, log_level=20, log_format='color', log_date_format=DateFormat.color, external_modules=None, external_packages=None, \*args, \*\*kwargs)

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



#### entrypoint()
Entrypoint instance.


* **Returns**

    An `Entrypoint` instance.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[[`minos.common.configuration.config.MinosConfig`](minos.common.configuration.config.md#minos.common.configuration.config.MinosConfig), `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= [`minos.common.setup.MinosSetup`](minos.common.setup.md#minos.common.setup.MinosSetup))



* **Returns**

    A instance of the called class.



#### graceful_shutdown(err=None)
Shutdown the services execution gracefully.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### injector()
Dependency injector instance.


* **Returns**

    A `DependencyInjector` instance.



#### launch()
Launch a new execution and keeps running forever..


* **Return type**

    `typing.NoReturn`



* **Returns**

    This method does not return anything.



#### loop()
Create the loop.


* **Returns**

    An `AbstractEventLoop` instance.



#### services()
List of services to be launched.


* **Returns**

    A list of `Service` instances.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
