# minos.saga.executions.steps.remote module


### _class_ minos.saga.executions.steps.remote.RemoteSagaStepExecution(definition, related_services=None, status=SagaStepStatus.Created, already_rollback=False)
Bases: [`minos.saga.executions.steps.abc.SagaStepExecution`](minos.saga.executions.steps.abc.md#minos.saga.executions.steps.abc.SagaStepExecution)

Saga Execution Step class.


#### \__init__(definition, related_services=None, status=SagaStepStatus.Created, already_rollback=False)

#### definition(_: [minos.saga.definitions.steps.remote.RemoteSagaStep](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep_ )

#### _async_ execute(context, response=None, \*args, \*\*kwargs)
Execution the remote step.


* **Parameters**

    
    * **context** ([`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)) – The execution context to be used during the execution.


    * **response** (`typing.Optional`[[`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse)]) – An optional command response instance (to be consumed by the on_success method).


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)



* **Returns**

    The updated context.



#### _static_ from_definition(step)
Build a `SagaStepExecution` instance from the `SagaStep` definition.


* **Parameters**

    **step** ([`minos.saga.definitions.steps.abc.SagaStep`](minos.saga.definitions.steps.abc.md#minos.saga.definitions.steps.abc.SagaStep)) – The `SagaStep` definition.



* **Return type**

    [`minos.saga.executions.steps.abc.SagaStepExecution`](minos.saga.executions.steps.abc.md#minos.saga.executions.steps.abc.SagaStepExecution)



* **Returns**

    A new `SagaStepExecution`.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from a raw representation.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], [`minos.saga.executions.steps.abc.SagaStepExecution`](minos.saga.executions.steps.abc.md#minos.saga.executions.steps.abc.SagaStepExecution)]) – The raw representation of the instance.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.executions.steps.abc.SagaStepExecution`](minos.saga.executions.steps.abc.md#minos.saga.executions.steps.abc.SagaStepExecution)



* **Returns**

    A `SagaStepExecution` instance.



#### _property_ raw(_: dict[str, Any_ )
Compute a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### _async_ rollback(context, \*args, \*\*kwargs)
Revert the executed remote step.


* **Parameters**

    
    * **context** ([`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)) – Execution context.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)



* **Returns**

    The updated execution context.
