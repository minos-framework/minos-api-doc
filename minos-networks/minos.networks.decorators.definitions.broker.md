# minos.networks.decorators.definitions.broker module


### _class_ minos.networks.decorators.definitions.broker.BrokerCommandEnrouteDecorator(topic)
Bases: `minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator`

Broker Command Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ _ = _ )

#### \__init__(topic)

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



### _class_ minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator(topic)
Bases: [`minos.networks.decorators.definitions.abc.EnrouteDecorator`](minos.networks.decorators.definitions.abc.md#minos.networks.decorators.definitions.abc.EnrouteDecorator), `abc.ABC`

Broker Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ )

#### \__init__(topic)

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



### _class_ minos.networks.decorators.definitions.broker.BrokerEventEnrouteDecorator(topic)
Bases: `minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator`

Broker Event Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ _ = _ )

#### \__init__(topic)

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



### _class_ minos.networks.decorators.definitions.broker.BrokerQueryEnrouteDecorator(topic)
Bases: `minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator`

Broker Query Enroute class


#### KIND(_: Final[[minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind](minos.networks.decorators.definitions.kinds.md#minos.networks.decorators.definitions.kinds.EnrouteDecoratorKind)_ _ = _ )

#### \__init__(topic)

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
