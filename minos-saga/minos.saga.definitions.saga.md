# minos.saga.definitions.saga module


### _class_ minos.saga.definitions.saga.Saga(\*args, steps=None, committed=False, commit=None, \*\*kwargs)
Bases: `object`

Saga class.

The purpose of this class is to define a sequence of operations among microservices.


#### \__init__(\*args, steps=None, committed=False, commit=None, \*\*kwargs)

#### commit(callback=None, \*\*kwargs)
Commit the instance to be ready for execution.


* **Parameters**

    
    * **callback** (`None`) – Deprecated argument.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.definitions.saga.Saga`



* **Returns**

    A `Saga` instance.



#### conditional_step(step=None)
Add a new conditional step.


* **Parameters**

    **step** (`typing.Optional`[[`minos.saga.definitions.steps.conditional.ConditionalSagaStep`](minos.saga.definitions.steps.conditional.md#minos.saga.definitions.steps.conditional.ConditionalSagaStep)]) – The step to be added. If None is provided then a new one will be created.



* **Return type**

    [`minos.saga.definitions.steps.conditional.ConditionalSagaStep`](minos.saga.definitions.steps.conditional.md#minos.saga.definitions.steps.conditional.ConditionalSagaStep)



* **Returns**

    A `SagaStep` instance.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new `Saga` instance from raw.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.definitions.saga.Saga`]) – The raw representation of the saga.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.definitions.saga.Saga`



* **Returns**

    A new `Saga` instance.



#### local_step(step=None, \*\*kwargs)
Add a new local step.


* **Parameters**

    
    * **step** (`typing.Union`[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `None`, `typing.Awaitable`[`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]]]], [`minos.saga.definitions.operations.SagaOperation`](minos.saga.definitions.operations.md#minos.saga.definitions.operations.SagaOperation)[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `None`, `typing.Awaitable`[`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]]]]], [`minos.saga.definitions.steps.local.LocalSagaStep`](minos.saga.definitions.steps.local.md#minos.saga.definitions.steps.local.LocalSagaStep), `None`]) – The step to be added. If None is provided then a new one will be created.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.local.LocalSagaStep`](minos.saga.definitions.steps.local.md#minos.saga.definitions.steps.local.LocalSagaStep)



* **Returns**

    A `SagaStep` instance.



#### _property_ raw(_: dict[str, Any_ )
Generate a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### remote_step(step=None, \*\*kwargs)
Add a new remote step step.


* **Parameters**

    
    * **step** (`typing.Union`[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]], [`minos.saga.definitions.operations.SagaOperation`](minos.saga.definitions.operations.md#minos.saga.definitions.operations.SagaOperation)[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]]], [`minos.saga.definitions.steps.remote.RemoteSagaStep`](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep), `None`]) – The step to be added. If None is provided then a new one will be created.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.remote.RemoteSagaStep`](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep)



* **Returns**

    A `SagaStep` instance.



#### step(step=None, \*\*kwargs)
Add a new remote step step.


* **Parameters**

    
    * **step** (`typing.Union`[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]], [`minos.saga.definitions.operations.SagaOperation`](minos.saga.definitions.operations.md#minos.saga.definitions.operations.SagaOperation)[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]]], [`minos.saga.definitions.steps.remote.RemoteSagaStep`](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep), `None`]) – The step to be added. If None is provided then a new one will be created.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.remote.RemoteSagaStep`](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep)



* **Returns**

    A `SagaStep` instance.



#### validate()
Check if the saga is valid.


* **Return type**

    `None`



* **Returns**

    This method does not return anything, but raises an exception if the saga is not valid.
