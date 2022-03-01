# minos.aggregate.events.entries module


### _class_ minos.aggregate.events.entries.EventEntry(uuid, name, version=None, data=b'', id=None, action=None, created_at=None, transaction_uuid=UUID('00000000-0000-0000-0000-000000000000'))
Bases: `object`

Class that represents an entry (or row) on the event repository database which stores the root entity changes.


#### \__init__(uuid, name, version=None, data=b'', id=None, action=None, created_at=None, transaction_uuid=UUID('00000000-0000-0000-0000-000000000000'))

#### action()

#### as_raw()
Get a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A dictionary in which the keys are attribute names and values the attribute contents.



#### created_at()

#### data()

#### _property_ event(_: [minos.aggregate.events.models.Event](minos.aggregate.events.models.md#minos.aggregate.events.models.Event_ )
Get the stored `Event` instance.


* **Return type**

    [`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event)



* **Returns**

    An `Event` instance.



#### _property_ field_diff_container(_: [minos.aggregate.events.fields.FieldDiffContainer](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiffContainer_ )
Get the stored field diff container.


* **Return type**

    [`minos.aggregate.events.fields.FieldDiffContainer`](minos.aggregate.events.fields.md#minos.aggregate.events.fields.FieldDiffContainer)



* **Returns**

    A `FieldDiffContainer` instance.



#### _classmethod_ from_another(another, \*\*kwargs)
Build a new instance from another `EventEntry`.


* **Parameters**

    
    * **another** (`minos.aggregate.events.entries.EventEntry`) – The `EventEntry`.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.aggregate.events.entries.EventEntry`



* **Returns**

    A new `EventEntry` instance.



#### _classmethod_ from_event(event, \*, transaction=None, \*\*kwargs)
Build a new instance from a `RootEntity`.


* **Parameters**

    
    * **event** ([`minos.aggregate.events.models.Event`](minos.aggregate.events.models.md#minos.aggregate.events.models.Event)) – The event.


    * **transaction** (`typing.Optional`[[`minos.aggregate.transactions.entries.TransactionEntry`](minos.aggregate.transactions.entries.md#minos.aggregate.transactions.entries.TransactionEntry)]) – Optional transaction.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.aggregate.events.entries.EventEntry`



* **Returns**

    A new `EventEntry` instance.



#### id()

#### name()

#### transaction_uuid()

#### _property_ type_(_: type[[minos.aggregate.entities.models.RootEntity](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)_ )
Load the concrete `RootEntity` class.


* **Return type**

    `type`[[`minos.aggregate.entities.models.RootEntity`](minos.aggregate.entities.models.md#minos.aggregate.entities.models.RootEntity)]



* **Returns**

    A `Type` object.



#### uuid()

#### version()
