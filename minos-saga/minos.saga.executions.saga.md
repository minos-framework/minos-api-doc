# minos.saga.executions.saga module


### _class_ minos.saga.executions.saga.SagaExecution(definition, uuid, context, status=SagaStatus.Created, steps=None, paused_step=None, already_rollback=False, user=None, \*args, \*\*kwargs)
Bases: `object`

Saga Execution class.


#### \__init__(definition, uuid, context, status=SagaStatus.Created, steps=None, paused_step=None, already_rollback=False, user=None, \*args, \*\*kwargs)

#### _async_ commit(\*args, \*\*kwargs)
Commit the execution transactions.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ execute(response=None, \*args, autocommit=True, \*\*kwargs)
Execute the `Saga` definition.


* **Parameters**

    
    * **response** (`typing.Optional`[[`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse)]) – An optional `SagaResponse` to be consumed by the immediately next executed step.


    * **args** – Additional positional arguments.


    * **autocommit** (`bool`) – If `True` the commit process is performed automatically, otherwise must be performed
    manually.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)



* **Returns**

    A 

    ```
    ``
    ```

    SagaContext instance.



#### _classmethod_ from_definition(definition, context=None, uuid=None, \*args, \*\*kwargs)
Build a new instance from a `Saga` object.


* **Parameters**

    
    * **definition** ([`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)) – The definition of the saga.


    * **context** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – Initial saga execution context. If not provided, then a new empty context is created.


    * **uuid** (`typing.Optional`[`uuid.UUID`]) – The identifier of the execution. If `None` is provided, then a new one will be generated.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.executions.saga.SagaExecution`



* **Returns**

    A new `SagaExecution` instance.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from a raw representation.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.executions.saga.SagaExecution`]) – The raw representation of the instance.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.executions.saga.SagaExecution`



* **Returns**

    A `SagaExecution` instance.



#### _classmethod_ from_saga(definition, context=None, \*args, \*\*kwargs)
Build a new instance from a `Saga` object.


* **Parameters**

    
    * **definition** ([`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)) – The definition of the saga.


    * **context** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – Initial saga execution context. If not provided, then a new empty context is created.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.executions.saga.SagaExecution`



* **Returns**

    A new `SagaExecution` instance.



#### _property_ raw(_: dict[str, Any_ )
Compute a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### _async_ reject(\*args, \*\*kwargs)
Reject the execution transactions.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ rollback(\*args, autoreject=True, \*\*kwargs)
Revert the executed operation with a compensatory operation.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **autoreject** (`bool`) – If `True` the commit process is performed automatically, otherwise must be performed
    manually.


    * **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    The updated execution context.
