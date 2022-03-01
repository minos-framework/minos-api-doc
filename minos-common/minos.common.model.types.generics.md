# minos.common.model.types.generics module


### _class_ minos.common.model.types.generics.GenericTypeProjector(type_hints, mapper)
Bases: `object`

Generic Type Projector.


#### \__init__(type_hints, mapper)

#### build()
Builder a projection of type vars values.


* **Return type**

    `dict`[`str`, `type`]



* **Returns**

    A dict of type hints.



#### _classmethod_ from_model(type_)
Build a new instance from model.


* **Parameters**

    **type** – The model class.



* **Return type**

    `minos.common.model.types.generics.GenericTypeProjector`



* **Returns**

    A `GenericTypeProjector` instance.



### minos.common.model.types.generics.unpack_typevar(value)
Unpack TypeVar into a union of possible types.


* **Parameters**

    **value** (`typing.TypeVar`(`TypeVar`, bound= <member ‘__bound__’ of ‘TypeVar’ objects>, covariant=<member ‘__covariant__’ of ‘TypeVar’ objects>, contravariant=<member ‘__contravariant__’ of ‘TypeVar’ objects>)) – A type var instance.



* **Return type**

    `type`



* **Returns**

    A union of types.
