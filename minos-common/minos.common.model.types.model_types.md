# minos.common.model.types.model_types module


### _class_ minos.common.model.types.model_types.FieldType(name: str, type: type)
Bases: `NamedTuple`

Field Type class.


#### count(value, /)
Return number of occurrences of value.


#### index(value, start=0, stop=9223372036854775807, /)
Return first index of value.

Raises ValueError if the value is not present.


#### name(_: st_ )
Alias for field number 0


#### type(_: typ_ )
Alias for field number 1


### _class_ minos.common.model.types.model_types.ModelType()
Bases: `type`

Model Type class.


#### \__init__(\*args, \*\*kwargs)

#### _classmethod_ build(name_, type_hints_=None, \*, namespace_=None, \*\*kwargs)
Build a new `ModelType` instance.


* **Parameters**

    
    * **name** – Name of the new type.


    * **type_hints** – Type hints of the new type.


    * **namespace** – Namespace of the new type.


    * **kwargs** – Type hints of the new type as named parameters.



* **Return type**

    `minos.common.model.types.model_types.ModelType`



* **Returns**

    A `ModelType` instance.



#### _property_ classname(_: st_ )
Get the full class name.


* **Return type**

    `str`



* **Returns**

    An string object.



#### _static_ from_model(type_)
Build a new instance from model class.


* **Parameters**

    **type** – The model class.



* **Return type**

    `minos.common.model.types.model_types.ModelType`



* **Returns**

    A new `ModelType` instance.



#### _classmethod_ from_typed_dict(typed_dict)
Build a new `ModelType` instance from a `typing.TypedDict`.


* **Parameters**

    **typed_dict** – Typed dict to be used as base.



* **Return type**

    `minos.common.model.types.model_types.ModelType`



* **Returns**

    A `ModelType` instance.



#### _property_ model_cls(_: Type[[minos.common.model.abc.Model](minos.common.model.abc.md#minos.common.model.abc.Model)_ )
Get the model class if defined or `DataTransferObject` otherwise.


* **Return type**

    `typing.Type`[[`minos.common.model.abc.Model`](minos.common.model.abc.md#minos.common.model.abc.Model)]



* **Returns**

    A model class.



#### mro()
Return a type’s method resolution order.


#### _property_ name(_: st_ )
Get the type name.


* **Return type**

    `str`



* **Returns**

    A string object.



#### namespace(_: st_ )

#### type_hints(_: dict[str, Type_ )
