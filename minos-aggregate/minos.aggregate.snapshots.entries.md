# minos.aggregate.snapshots.entries module


### _class_ minos.aggregate.snapshots.entries.SnapshotEntry(uuid, name, version, schema=None, data=None, created_at=None, updated_at=None, transaction_uuid=UUID('00000000-0000-0000-0000-000000000000'))
Bases: `object`

Minos Snapshot Entry class.

Is the python object representation of a row in the `snapshot` storage system.


#### \__init__(uuid, name, version, schema=None, data=None, created_at=None, updated_at=None, transaction_uuid=UUID('00000000-0000-0000-0000-000000000000'))

#### as_raw()
Get a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A dictionary in which the keys are attribute names and values the attribute contents.



#### build(\*\*kwargs)
Rebuild the stored `RootEntity` object instance from the internal state.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    [`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)



* **Returns**

    A `RootEntity` instance.



#### created_at()

#### data()

#### _property_ encoded_data(_: Optional[str_ )
Get the encoded data if available.


* **Return type**

    `typing.Optional`[`str`]



* **Returns**

    A `str` instance or `None`.



#### _property_ encoded_schema(_: Optional[bytes_ )
Get the encoded schema if available.


* **Return type**

    `typing.Optional`[`bytes`]



* **Returns**

    A `bytes` instance or `None`.



#### _classmethod_ from_event_entry(entry)
Build a new `SnapshotEntry` from a deletion event.


* **Parameters**

    **entry** ([`minos.aggregate.events.entries.EventEntry`](minos.aggregate.events.entries.md#minos.aggregate.events.entries.EventEntry)) – The event entry containing the delete information.



* **Return type**

    `minos.aggregate.snapshots.entries.SnapshotEntry`



* **Returns**

    A new `SnapshotEntry` instance.



#### _classmethod_ from_root_entity(instance, \*\*kwargs)
Build a new instance from a `RootEntity`.


* **Parameters**

    **instance** ([`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)) – The `RootEntity` instance.



* **Return type**

    `minos.aggregate.snapshots.entries.SnapshotEntry`



* **Returns**

    A new `SnapshotEntry` instance.



#### name()

#### schema()

#### transaction_uuid()

#### _property_ type_(_: type[[minos.aggregate.entities.models.RootEntity](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)_ )
Load the concrete `RootEntity` class.


* **Return type**

    `type`[[`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)]



* **Returns**

    A `Type` object.



#### updated_at()

#### uuid()

#### version()
