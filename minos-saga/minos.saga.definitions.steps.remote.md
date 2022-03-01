# minos.saga.definitions.steps.remote module


### _class_ minos.saga.definitions.steps.remote.RemoteSagaStep(on_execute=None, on_success=None, on_error=None, on_failure=None, \*\*kwargs)
Bases: [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)

Remote Saga Step class.


#### \__init__(on_execute=None, on_success=None, on_error=None, on_failure=None, \*\*kwargs)

#### commit(\*args, \*\*kwargs)
Commit the current `SagaStep` on the `Saga`.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)



* **Returns**

    A `Saga` instance.



#### conditional_step(\*args, \*\*kwargs)
Create a new conditional step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.conditional.ConditionalSagaStep`](minos.saga.definitions.steps.conditional.md#minos.saga.definitions.steps.conditional.ConditionalSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from raw.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)]) – A raw representation.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)



* **Returns**

    A `SagaStep` instance.



#### local_step(\*args, \*\*kwargs)
Create a new local step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.local.LocalSagaStep`](minos.saga.definitions.steps.local.md#minos.saga.definitions.steps.local.LocalSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### on_error(callback, parameters=None, \*\*kwargs)
On error method.


* **Parameters**

    
    * **callback** (`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), [`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse), `...`, `typing.Union`[`Exception`, [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `typing.Awaitable`[`typing.Union`[`Exception`, [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]]]]) – The callback function to be called.


    * **parameters** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – A mapping of named parameters to be passed to the callback.


    * **kwargs** – A set of named arguments to be passed to the callback. `parameters` has priority if it is not
    `None`.



* **Return type**

    `minos.saga.definitions.steps.remote.RemoteSagaStep`



* **Returns**

    A `self` reference.



#### on_execute(callback, parameters=None, \*\*kwargs)
On execute method.


* **Parameters**

    
    * **callback** (`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]]) – The callback function to be called.


    * **parameters** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – A mapping of named parameters to be passed to the callback.


    * **kwargs** – A set of named arguments to be passed to the callback. `parameters` has priority if it is not
    `None`.



* **Return type**

    `minos.saga.definitions.steps.remote.RemoteSagaStep`



* **Returns**

    A `self` reference.



#### on_failure(callback, parameters=None, \*\*kwargs)
On failure method.


* **Parameters**

    
    * **callback** (`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]]) – The callback function to be called.


    * **parameters** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – A mapping of named parameters to be passed to the callback.


    * **kwargs** – A set of named arguments to be passed to the callback. `parameters` has priority if it is not
    `None`.



* **Return type**

    `minos.saga.definitions.steps.remote.RemoteSagaStep`



* **Returns**

    A `self` reference.



#### on_success(callback, parameters=None, \*\*kwargs)
On success method.


* **Parameters**

    
    * **callback** (`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), [`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse), `...`, `typing.Union`[`Exception`, [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `typing.Awaitable`[`typing.Union`[`Exception`, [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]]]]) – The callback function to be called.


    * **parameters** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – A mapping of named parameters to be passed to the callback.


    * **kwargs** – A set of named arguments to be passed to the callback. `parameters` has priority if it is not
    `None`.



* **Return type**

    `minos.saga.definitions.steps.remote.RemoteSagaStep`



* **Returns**

    A `self` reference.



#### _property_ raw(_: dict[str, Any_ )
Generate a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### remote_step(\*args, \*\*kwargs)
Create a new remote step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    `minos.saga.definitions.steps.remote.RemoteSagaStep`



* **Returns**

    A new `SagaStep` instance.



#### step(\*args, \*\*kwargs)
Create a new step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)



* **Returns**

    A new `SagaStep` instance.



#### validate()
Check if the step is valid.


* **Return type**

    `None`



* **Returns**

    This method does not return anything, but raises an exception if the step is not valid.
