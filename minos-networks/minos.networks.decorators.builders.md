# minos.networks.decorators.builders module


### _class_ minos.networks.decorators.builders.EnrouteBuilder(\*classes, middleware=None)
Bases: `object`

Enroute builder class.


#### \__init__(\*classes, middleware=None)

#### get_broker_command_query(\*\*kwargs)
Get the broker actions for commands and queries.


* **Return type**

    `dict`[[`minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator`](minos.networks.decorators.definitions.broker.md#minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator), `collections.abc.Callable`[[`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request), `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]]



* **Returns**

    A dictionary with decorator classes as keys and callable actions as values.



#### get_broker_command_query_event(\*\*kwargs)
Get the broker actions for commands, queries and events.


* **Return type**

    `dict`[[`minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator`](minos.networks.decorators.definitions.broker.md#minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator), `collections.abc.Callable`[[`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request), `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]]



* **Returns**

    A dictionary with decorator classes as keys and callable actions as values.



#### get_broker_event(\*\*kwargs)
Get the broker actions for events.


* **Return type**

    `dict`[[`minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator`](minos.networks.decorators.definitions.broker.md#minos.networks.decorators.definitions.broker.BrokerEnrouteDecorator), `collections.abc.Callable`[[`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request), `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]]



* **Returns**

    A dictionary with decorator classes as keys and callable actions as values.



#### get_periodic_event(\*\*kwargs)
Get the periodic actions for events.


* **Return type**

    `dict`[[`minos.networks.decorators.definitions.periodic.PeriodicEnrouteDecorator`](minos.networks.decorators.definitions.periodic.md#minos.networks.decorators.definitions.periodic.PeriodicEnrouteDecorator), `collections.abc.Callable`[[`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request), `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]]



* **Returns**

    A dictionary with decorator classes as keys and callable actions as values.



#### get_rest_command_query(\*\*kwargs)
Get the rest actions for commands and queries.


* **Return type**

    `dict`[[`minos.networks.decorators.definitions.rest.RestEnrouteDecorator`](minos.networks.decorators.definitions.rest.md#minos.networks.decorators.definitions.rest.RestEnrouteDecorator), `collections.abc.Callable`[[`minos.networks.requests.abc.Request`](minos.networks.requests.abc.md#minos.networks.requests.abc.Request), `collections.abc.Awaitable`[`typing.Optional`[[`minos.networks.requests.abc.Response`](minos.networks.requests.abc.md#minos.networks.requests.abc.Response)]]]]



* **Returns**

    A dictionary with decorator classes as keys and callable actions as values.
