# minos.aggregate.transactions.entries module


### _class_ minos.aggregate.transactions.entries.TransactionEntry(uuid=None, status=None, event_offset=None, destination_uuid=None, updated_at=None, autocommit=True, event_repository=<dependency_injector.wiring.Provide object>, transaction_repository=<dependency_injector.wiring.Provide object>)
Bases: `object`

Transaction Entry class.


#### \__init__(uuid=None, status=None, event_offset=None, destination_uuid=None, updated_at=None, autocommit=True, event_repository=<dependency_injector.wiring.Provide object>, transaction_repository=<dependency_injector.wiring.Provide object>)

#### _async_ commit()
Commit transaction changes.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _property_ destination(_: Optional[minos.aggregate.transactions.entries.TransactionEntry_ )
Get the destination transaction if there is anyone, otherwise `None` is returned.


* **Return type**

    `typing.Optional`[`minos.aggregate.transactions.entries.TransactionEntry`]



* **Returns**

    A `TransactionEntry` or `None`.



#### destination_uuid()

#### event_offset()

#### _async_ reject()
Reject transaction changes.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ reserve()
Reserve transaction changes to be ensured that they can be applied.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ save(\*, event_offset=None, status=None)
Saves the transaction into the repository.


* **Parameters**

    
    * **event_offset** (`typing.Optional`[`int`]) – The event offset.


    * **status** (`typing.Optional`[`minos.aggregate.transactions.entries.TransactionStatus`]) – The status.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### status()

#### updated_at()

#### uuid()

#### _property_ uuids(_: tuple[uuid.UUID, ..._ )
Get the sequence of transaction identifiers, from the outer one (`NULL_UUID`) to the one related with self.


* **Return type**

    `tuple`[`uuid.UUID`, `...`]



* **Returns**

    A tuple of `UUID` values.



#### _async_ validate()
Check if the transaction is committable.


* **Return type**

    `bool`



* **Returns**

    `True` if the transaction is valid or `False` otherwise.



### _class_ minos.aggregate.transactions.entries.TransactionStatus(value)
Bases: `str`, `enum.Enum`

Transaction Status Enum.


#### COMMITTED(_ = 'committed_ )

#### COMMITTING(_ = 'committing_ )

#### PENDING(_ = 'pending_ )

#### REJECTED(_ = 'rejected_ )

#### RESERVED(_ = 'reserved_ )

#### RESERVING(_ = 'reserving_ )

#### _classmethod_ value_of(value)
Get the status based on its text representation.


* **Return type**

    `minos.aggregate.transactions.entries.TransactionStatus`
