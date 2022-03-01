# minos.common.model.types.builders module


### _class_ minos.common.model.types.builders.TypeHintBuilder(value, type_=None)
Bases: `object`

Type Hint Builder class.


#### \__init__(value, type_=None)

#### build()
Build type hint from an instance..


* **Return type**

    `type`



* **Returns**

    A type.



### minos.common.model.types.builders.build_union(options)
Build the union type base on the given options.


* **Parameters**

    **options** (`collections.abc.Iterable`[`type`, `...`]) – A tuple of types.



* **Return type**

    `type`



* **Returns**

    The union of types.
