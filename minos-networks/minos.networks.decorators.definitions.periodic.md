# minos.networks.decorators.definitions.periodic module


### _class_ minos.networks.decorators.definitions.periodic.PeriodicEnrouteDecorator(crontab)
Bases: [`minos.networks.decorators.definitions.abc.EnrouteDecorator`](minos.networks.decorators.definitions.abc.md#minos.networks.decorators.definitions.abc.EnrouteDecorator), `abc.ABC`

Periodic Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ )

#### \__init__(crontab)

#### _property_ post_fn_name(_: st_ )
Get the post execution function name.


* **Return type**

    `str`



* **Returns**

    A string value containing the function name.



#### _property_ pre_fn_name(_: st_ )
Get the pre execution function name.


* **Return type**

    `str`



* **Returns**

    A string value containing the function name.



### _class_ minos.networks.decorators.definitions.periodic.PeriodicEventEnrouteDecorator(crontab)
Bases: `minos.networks.decorators.definitions.periodic.PeriodicEnrouteDecorator`

Periodic Event Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ _ = _ )

#### \__init__(crontab)

#### _property_ post_fn_name(_: st_ )
Get the post execution function name.


* **Return type**

    `str`



* **Returns**

    A string value containing the function name.



#### _property_ pre_fn_name(_: st_ )
Get the pre execution function name.


* **Return type**

    `str`



* **Returns**

    A string value containing the function name.
