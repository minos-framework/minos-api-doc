# minos.aggregate.actions module


### _class_ minos.aggregate.actions.Action(value)
Bases: `str`, `enum.Enum`

Enum class that describes the actions.


#### CREATE(_ = 'create_ )

#### DELETE(_ = 'delete_ )

#### UPDATE(_ = 'update_ )

#### _property_ is_create(_: boo_ )
Check if the action is create.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _property_ is_delete(_: boo_ )
Check if the action is create.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _property_ is_update(_: boo_ )
Check if the action is create.


* **Return type**

    `bool`



* **Returns**

    A boolean value.



#### _classmethod_ value_of(value)
Get the action based on its text representation.


* **Return type**

    `minos.aggregate.actions.Action`
