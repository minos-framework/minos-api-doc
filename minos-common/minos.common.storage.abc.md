# minos.common.storage.abc module


### _class_ minos.common.storage.abc.MinosStorage()
Bases: `abc.ABC`

Minos Storage interface.


#### _abstract_ add(\*\*kwargs)
Store a value.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _abstract classmethod_ build(\*\*kwargs)
Build a new instance.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `minos.common.storage.abc.MinosStorage`



* **Returns**

    A new `MinosStorage` instance.



#### _abstract_ delete(\*\*kwargs)
Delete the stored value.


* **Parameters**

    **kwargs** – 



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _abstract_ get(\*\*kwargs)
Get the stored value..


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `typing.Optional`[`typing.Any`]



* **Returns**

    The stored value.



#### _abstract_ update(\*\*kwargs)
Update the stored value.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.
