# minos.saga.executions.steps.abc module


### _class_ minos.saga.executions.steps.abc.SagaStepExecution(definition, related_services=None, status=SagaStepStatus.Created, already_rollback=False)
Bases: `abc.ABC`

Saga Step Execution class.


#### \__init__(definition, related_services=None, status=SagaStepStatus.Created, already_rollback=False)

#### _abstract async_ execute(context, \*args, \*\*kwargs)
Execution the step.


* **Parameters**

    
    * **context** ([`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)) – The execution context to be used during the execution.


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

    `minos.saga.executions.steps.abc.SagaStepExecution`



* **Returns**

    A new `SagaStepExecution`.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from a raw representation.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.executions.steps.abc.SagaStepExecution`]) – The raw representation of the instance.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.executions.steps.abc.SagaStepExecution`



* **Returns**

    A `SagaStepExecution` instance.



#### _property_ raw(_: dict[str, Any_ )
Compute a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### _abstract async_ rollback(context, \*args, \*\*kwargs)
Revert the executed step.


* **Parameters**

    
    * **context** ([`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)) – Execution context.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)



* **Returns**

    The updated execution context.
