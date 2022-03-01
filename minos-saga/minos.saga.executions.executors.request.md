# minos.saga.executions.executors.request module


### _class_ minos.saga.executions.executors.request.RequestExecutor(\*args, user, broker_publisher=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Bases: [`minos.saga.executions.executors.abc.Executor`](minos.saga.executions.executors.abc.md#minos.saga.executions.executors.abc.Executor)

Request Executor class.

This class has the responsibility to publish command on the corresponding broker’s queue.


#### \__init__(\*args, user, broker_publisher=<dependency_injector.wiring.Provide object>, \*\*kwargs)

#### _async_ exec(operation, context)
Exec method, that perform the publishing logic run an pre-callback function to generate the command contents.


* **Parameters**

    
    * **operation** (`typing.Optional`[[`minos.saga.definitions.operations.SagaOperation`](minos.saga.definitions.operations.md#minos.saga.definitions.operations.SagaOperation)[`collections.abc.Callable`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext), `...`, `typing.Union`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest), `typing.Awaitable`[[`minos.saga.messages.SagaRequest`](minos.saga.messages.md#minos.saga.messages.SagaRequest)]]]]]) – Operation to be executed.


    * **context** ([`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)) – Execution context.



* **Return type**

    [`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)



* **Returns**

    A saga context instance.



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
