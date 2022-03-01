# minos.saga.executions.executors.abc module


### _class_ minos.saga.executions.executors.abc.Executor(execution_uuid, \*args, \*\*kwargs)
Bases: `object`

Executor class.


#### \__init__(execution_uuid, \*args, \*\*kwargs)

#### _async_ exec(operation, \*args, \*\*kwargs)
Execute the given operation.


* **Parameters**

    
    * **operation** ([`minos.saga.definitions.operations.SagaOperation`](minos.saga.definitions.operations.md#minos.saga.definitions.operations.SagaOperation)) – The operation to be executed.


    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Any`



* **Returns**

    The execution response.



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
