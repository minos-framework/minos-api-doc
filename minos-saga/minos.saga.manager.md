# minos.saga.manager module


### _class_ minos.saga.manager.SagaManager(storage, broker_pool=<dependency_injector.wiring.Provide object>, \*args, \*\*kwargs)
Bases: `minos.common.setup.MinosSetup`

Saga Manager implementation class.

The purpose of this class is to manage the running process for new or paused\`\`SagaExecution\`\` instances.


#### \__init__(storage, broker_pool=<dependency_injector.wiring.Provide object>, \*args, \*\*kwargs)

#### _property_ already_destroyed(_: boo_ )
Already Destroy getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _property_ already_setup(_: boo_ )
Already Setup getter.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _async_ destroy()
Destroy miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ run(definition=None, context=None, \*, response=None, user=None, autocommit=True, pause_on_disk=False, raise_on_error=True, return_execution=True, \*\*kwargs)
Perform a run of a `Saga`.

The run can be a new one (if a name is provided) or continue execution a previous one (if a reply is provided).


* **Parameters**

    
    * **definition** (`typing.Optional`[[`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)]) – Saga definition to be executed.


    * **context** (`typing.Optional`[[`minos.saga.context.SagaContext`](minos.saga.context.md#minos.saga.context.SagaContext)]) – Initial context to be used during the execution. (Only used for new executions)


    * **response** (`typing.Optional`[[`minos.saga.messages.SagaResponse`](minos.saga.messages.md#minos.saga.messages.SagaResponse)]) – The reply that relaunches a saga execution.


    * **user** (`typing.Optional`[`uuid.UUID`]) – The user identifier to be injected on remote steps.


    * **autocommit** (`bool`) – If `True` the transactions are committed/rejected automatically. Otherwise, the `commit`
    or `reject` must to be called manually.


    * **pause_on_disk** (`bool`) – If `True` the pauses until remote steps’ responses are paused on disk (background,
    non-blocking the execution). Otherwise, the pauses are waited on memory (online, blocking the execution)


    * **raise_on_error** (`bool`) – If `True` exceptions are raised on error. Otherwise, the execution is returned normally
    but with `Errored` status.


    * **return_execution** (`bool`) – If `True` the `SagaExecution` instance is returned. Otherwise, only the
    identifier (`UUID`) is returned.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.Union`[`uuid.UUID`, [`minos.saga.executions.saga.SagaExecution`](minos.saga.executions.saga.md#minos.saga.executions.saga.SagaExecution)]



* **Returns**

    This method does not return anything.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.
