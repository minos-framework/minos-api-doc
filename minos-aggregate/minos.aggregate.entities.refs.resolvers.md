# minos.aggregate.entities.refs.resolvers module


### _class_ minos.aggregate.entities.refs.resolvers.RefResolver(broker_pool=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Bases: `object`

Ref Resolver class.


#### \__init__(broker_pool=<dependency_injector.wiring.Provide object>, \*\*kwargs)

#### _async_ resolve(data, \*\*kwargs)
Resolve Ref instances.


* **Parameters**

    
    * **data** (`typing.Any`) – The data to be resolved.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The data instance with model references already resolved.
