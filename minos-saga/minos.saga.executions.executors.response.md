# minos.saga.executions.executors.response module


### _class_ minos.saga.executions.executors.response.ResponseExecutor(execution_uuid, \*args, \*\*kwargs)
Bases: [`minos.saga.executions.executors.abc.Executor`](minos.saga.executions.executors.abc.md#minos.saga.executions.executors.abc.Executor)

Response Executor class.


#### \__init__(execution_uuid, \*args, \*\*kwargs)

#### _async_ exec(operation, context, response, \*args, \*\*kwargs)
Execute the operation.


* **Parameters**

    
    * **operation** (`typing.Optional`[[`minos.saga.definitions.operations.SagaOperation`](minos.saga.definitions.operations.md#minos.saga.definitions.operations.SagaOperation)[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), [`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse), `...`, `typing.Union`[`Exception`, [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `typing.Awaitable`[`typing.Union`[`Exception`, [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]]]]]]) – Operation to be executed.


    * **context** ([`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)) – Actual execution context.


    * **response** ([`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse)) – SagaResponse containing the response content.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)



* **Returns**

    An updated context instance.



#### _async_ exec_function(func, \*args, \*\*kwargs)
Execute a function.


* **Parameters**

    
    * **func** (`typing.Callable`) – Function to be executed.


    * **args** – Additional positional arguments to the function.


    * **kwargs** – Additional named arguments to the function.



* **Return type**

    `typing.Any`



* **Returns**

    The `func` result.
