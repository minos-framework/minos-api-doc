# minos.networks.decorators.definitions.rest module


### _class_ minos.networks.decorators.definitions.rest.RestCommandEnrouteDecorator(url, method)
Bases: `minos.networks.decorators.definitions.rest.RestEnrouteDecorator`

Rest Command Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ _ = _ )

#### \__init__(url, method)

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



### _class_ minos.networks.decorators.definitions.rest.RestEnrouteDecorator(url, method)
Bases: [`minos.networks.decorators.definitions.abc.EnrouteDecorator`](minos.networks.decorators.definitions.abc.md#minos.networks.decorators.definitions.abc.EnrouteDecorator), `abc.ABC`

Rest Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ )

#### \__init__(url, method)

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



### _class_ minos.networks.decorators.definitions.rest.RestQueryEnrouteDecorator(url, method)
Bases: `minos.networks.decorators.definitions.rest.RestEnrouteDecorator`

Rest Query Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ _ = _ )

#### \__init__(url, method)

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
