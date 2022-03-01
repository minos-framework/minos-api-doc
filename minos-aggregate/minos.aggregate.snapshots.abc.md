# minos.aggregate.snapshots.abc module


### _class_ minos.aggregate.snapshots.abc.SnapshotRepository(\*args, already_setup=False, \*\*kwargs)
Bases: `abc.ABC`, `minos.common.setup.MinosSetup`

Base Snapshot class.

The snapshot provides a direct accessor to the `RootEntity` instances stored as events by the event repository
class.


#### \__init__(\*args, already_setup=False, \*\*kwargs)

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



#### _async_ find(name, condition, ordering=None, limit=None, streaming_mode=False, transaction=None, \*\*kwargs)
Find a collection of `RootEntity` instances based on a `Condition`.


* **Parameters**

    
    * **name** (`str`) – Class name of the `RootEntity`.


    * **condition** (`minos.aggregate.queries._Condition`) – The condition that must be satisfied by the `RootEntity` instances.


    * **ordering** (`typing.Optional`[`minos.aggregate.queries._Ordering`]) – Optional argument to return the instance with specific ordering strategy. The default behaviour
    is to retrieve them without any order pattern.


    * **limit** (`typing.Optional`[`int`]) – Optional argument to return only a subset of instances. The default behaviour is to return all the
    instances that meet the given condition.


    * **streaming_mode** (`bool`) – If `True` return the values in streaming directly from the database (keep an open
    database connection), otherwise preloads the full set of values on memory and then retrieves them.


    * **transaction** (`typing.Optional`[[`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)]) – The transaction within the operation is performed. If not any value is provided, then the
    transaction is extracted from the context var. If not any transaction is being scoped then the query is
    performed to the global snapshot.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncIterator`[[`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)]



* **Returns**

    An asynchronous iterator that containing the `RootEntity` instances.



#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _async_ get(name, uuid, transaction=None, \*\*kwargs)
Get a `RootEntity` instance from its identifier.


* **Parameters**

    
    * **name** (`str`) – Class name of the `RootEntity`.


    * **uuid** (`uuid.UUID`) – Identifier of the `RootEntity`.


    * **transaction** (`typing.Optional`[[`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)]) – The transaction within the operation is performed. If not any value is provided, then the
    transaction is extracted from the context var. If not any transaction is being scoped then the query is
    performed to the global snapshot.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)



* **Returns**

    The `RootEntity` instance.



#### get_all(name, ordering=None, limit=None, streaming_mode=False, transaction=None, \*\*kwargs)
Get all `RootEntity` instances.


* **Parameters**

    
    * **name** (`str`) – Class name of the `RootEntity`.


    * **ordering** (`typing.Optional`[`minos.aggregate.queries._Ordering`]) – Optional argument to return the instance with specific ordering strategy. The default behaviour
    is to retrieve them without any order pattern.


    * **limit** (`typing.Optional`[`int`]) – Optional argument to return only a subset of instances. The default behaviour is to return all the
    instances that meet the given condition.


    * **streaming_mode** (`bool`) – If `True` return the values in streaming directly from the database (keep an open
    database connection), otherwise preloads the full set of values on memory and then retrieves them.


    * **transaction** (`typing.Optional`[[`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)]) – The transaction within the operation is performed. If not any value is provided, then the
    transaction is extracted from the context var. If not any transaction is being scoped then the query is
    performed to the global snapshot.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.AsyncIterator`[[`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)]



* **Returns**

    An asynchronous iterator that containing the `RootEntity` instances.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### synchronize(\*\*kwargs)
Synchronize the snapshot to the latest available version.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.Awaitable`[`None`]



* **Returns**

    This method does not return anything.
