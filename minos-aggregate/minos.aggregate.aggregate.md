# minos.aggregate.aggregate module


### _class_ minos.aggregate.aggregate.Aggregate(transaction_repository, event_repository, snapshot_repository, \*args, \*\*kwargs)
Bases: `Generic`[`minos.aggregate.aggregate.RT`], `minos.common.setup.MinosSetup`

Base Service class


#### \__init__(transaction_repository, event_repository, snapshot_repository, \*args, \*\*kwargs)

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



#### event_repository(_: [minos.aggregate.events.repositories.abc.EventRepository](minos.aggregate.events.repositories.abc.md#minos.aggregate.events.repositories.abc.EventRepository_ )

#### _classmethod_ from_config(config=None, \*\*kwargs)
Build a new instance from config.


* **Parameters**

    
    * **config** (`typing.Union`[`minos.common.configuration.config.MinosConfig`, `pathlib.Path`, `None`]) – Config instance. If None is provided, default config is chosen.


    * **kwargs** – Additional named arguments.



* **Return type**

    `typing.TypeVar`(`S`, bound= `minos.common.setup.MinosSetup`)



* **Returns**

    A instance of the called class.



#### _property_ root(_: type[[minos.aggregate.entities.models.RootEntity](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)_ )
Get the root entity of the aggregate.


* **Return type**

    `type`[[`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)]



* **Returns**

    A `RootEntity` type.



#### _async_ setup()
Setup miscellaneous repository things.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### snapshot_repository(_: [minos.aggregate.snapshots.abc.SnapshotRepository](minos.aggregate.snapshots.abc.md#minos.aggregate.snapshots.abc.SnapshotRepository_ )

#### transaction_repository(_: [minos.aggregate.transactions.repositories.abc.TransactionRepository](minos.aggregate.transactions.repositories.abc.md#minos.aggregate.transactions.repositories.abc.TransactionRepository_ )
