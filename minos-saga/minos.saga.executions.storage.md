# minos.saga.executions.storage module


### _class_ minos.saga.executions.storage.SagaExecutionStorage(storage_cls=<class 'minos.common.storage.lmdb.MinosStorageLmdb'>, protocol=<class 'minos.common.protocol.json.MinosJsonBinaryProtocol'>, db_name='LocalState', \*\*kwargs)
Bases: `object`

Saga Execution Storage class.


#### \__init__(storage_cls=<class 'minos.common.storage.lmdb.MinosStorageLmdb'>, protocol=<class 'minos.common.protocol.json.MinosJsonBinaryProtocol'>, db_name='LocalState', \*\*kwargs)

#### delete(key)
Delete the reference of the given key.


* **Parameters**

    **key** (`typing.Union`[[`minos.saga.executions.saga.SagaExecution`](minos.saga.executions.saga.md#minos.saga.executions.saga.SagaExecution), `str`, `uuid.UUID`]) – Execution key to be deleted.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _classmethod_ from_config(config, \*\*kwargs)
Build an instance from config.


* **Parameters**

    
    * **config** (`minos.common.configuration.config.MinosConfig`) – Config instance.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.executions.storage.SagaExecutionStorage`



* **Returns**

    A new `SagaExecutionStorage` instance.



#### load(key)
Load the saga execution stored on the given key.


* **Parameters**

    **key** (`typing.Union`[`str`, `uuid.UUID`]) – The key to identify the execution.



* **Return type**

    [`minos.saga.executions.saga.SagaExecution`](minos.saga.executions.saga.md#minos.saga.executions.saga.SagaExecution)



* **Returns**

    A `SagaExecution` instance.



#### store(execution)
Store an execution.


* **Parameters**

    **execution** ([`minos.saga.executions.saga.SagaExecution`](minos.saga.executions.saga.md#minos.saga.executions.saga.SagaExecution)) – Execution to be stored.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
