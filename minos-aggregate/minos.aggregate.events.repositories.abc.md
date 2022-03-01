# minos.aggregate.events.repositories.abc module


### _class_ minos.aggregate.events.repositories.abc.EventRepository(broker_publisher=<dependency_injector.wiring.Provide object>, transaction_repository=<dependency_injector.wiring.Provide object>, lock_pool=<dependency_injector.wiring.Provide object>, \*args, \*\*kwargs)
Bases: `abc.ABC`, `minos.common.setup.MinosSetup`

Base event repository class in `minos`.


#### \__init__(broker_publisher=<dependency_injector.wiring.Provide object>, transaction_repository=<dependency_injector.wiring.Provide object>, lock_pool=<dependency_injector.wiring.Provide object>, \*args, \*\*kwargs)

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



#### _async_ create(entry)
Store new creation entry into the repository.


* **Parameters**

    **entry** (`typing.Union`[[`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event), [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)]) – Entry to be stored.



* **Return type**

    [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)



* **Returns**

    The repository entry containing the stored information.



#### _async_ delete(entry)
Store new deletion entry into the repository.


* **Parameters**

    **entry** (`typing.Union`[[`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event), [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)]) – Entry to be stored.



* **Return type**

    [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)



* **Returns**

    The repository entry containing the stored information.



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



#### _property_ offset(_: Awaitable[int_ )
Get the current repository offset.


* **Return type**

    `typing.Awaitable`[`int`]



* **Returns**

    An awaitable containing an integer value.



#### _async_ select(uuid=None, name=None, version=None, version_lt=None, version_gt=None, version_le=None, version_ge=None, id=None, id_lt=None, id_gt=None, id_le=None, id_ge=None, transaction_uuid=None, transaction_uuid_ne=None, transaction_uuid_in=None, \*\*kwargs)
Perform a selection query of entries stored in to the repository.


* **Parameters**

    
    * **uuid** (`typing.Optional`[`uuid.UUID`]) – The identifier must be equal to the given value.


    * **name** (`typing.Optional`[`str`]) – The classname must be equal to the given value.


    * **version** (`typing.Optional`[`int`]) – The version must be equal to the given value.


    * **version_lt** (`typing.Optional`[`int`]) – The version must be lower than the given value.


    * **version_gt** (`typing.Optional`[`int`]) – The version must be greater than the given value.


    * **version_le** (`typing.Optional`[`int`]) – The version must be lower or equal to the given value.


    * **version_ge** (`typing.Optional`[`int`]) – The version must be greater or equal to the given value.


    * **id** (`typing.Optional`[`int`]) – The entry identifier must be equal to the given value.


    * **id_lt** (`typing.Optional`[`int`]) – The entry identifier must be lower than the given value.


    * **id_gt** (`typing.Optional`[`int`]) – The entry identifier must be greater than the given value.


    * **id_le** (`typing.Optional`[`int`]) – The entry identifier must be lower or equal to the given value.


    * **id_ge** (`typing.Optional`[`int`]) – The entry identifier must be greater or equal to the given value.


    * **transaction_uuid** (`typing.Optional`[`uuid.UUID`]) – The transaction identifier must be equal to the given value.


    * **transaction_uuid_ne** (`typing.Optional`[`uuid.UUID`]) – The transaction identifier must be distinct of the given value.


    * **transaction_uuid_in** (`typing.Optional`[`tuple`[`uuid.UUID`, `...`]]) – The destination transaction identifier must be equal to one of the given values.



* **Return type**

    `typing.AsyncIterator`[[`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)]



* **Returns**

    A list of entries.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ submit(entry, \*\*kwargs)
Store new entry into the repository.


* **Parameters**

    
    * **entry** (`typing.Union`[[`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event), [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)]) – The entry to be stored.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)



* **Returns**

    The repository entry containing the stored information.



#### transaction(\*\*kwargs)
Build a transaction instance related to the repository.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)



* **Returns**

    A new `TransactionEntry` instance.



#### _async_ update(entry)
Store new update entry into the repository.


* **Parameters**

    **entry** (`typing.Union`[[`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event), [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)]) – Entry to be stored.



* **Return type**

    [`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)



* **Returns**

    The repository entry containing the stored information.



#### _async_ validate(entry, transaction_uuid_ne=None, \*\*kwargs)
Check if it is able to submit the given entry.


* **Parameters**

    
    * **entry** ([`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)) – The entry to be validated.


    * **transaction_uuid_ne** (`typing.Optional`[`uuid.UUID`]) – Optional transaction identifier to skip it from the validation.


    * **kwargs** – Additional named arguments.



* **Return type**

    `bool`



* **Returns**

    `True` if the entry can be submitted or `False` otherwise.



#### write_lock()
Get a write lock.


* **Return type**

    `minos.common.locks.Lock`



* **Returns**

    An asynchronous context manager.
