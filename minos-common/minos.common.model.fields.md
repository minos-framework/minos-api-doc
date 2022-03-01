# minos.common.model.fields module


### _class_ minos.common.model.fields.Field(name, type_, value=<class 'minos.common.model.types.constants.MissingSentinel'>, parser=None, validator=None)
Bases: `object`

Represents a model field.


#### \__init__(name, type_, value=<class 'minos.common.model.types.constants.MissingSentinel'>, parser=None, validator=None)

#### _property_ avro_data(_: An_ )
Compute the avro data of the model.


* **Return type**

    `typing.Any`



* **Returns**

    A dictionary object.



#### _property_ avro_schema(_: dict[str, Any_ )
Compute the avro schema of the field.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A dictionary object.



#### _classmethod_ from_avro(schema, value)
Build a `Field` instance from the avro information.


* **Parameters**

    
    * **schema** (`dict`) – Field’s schema.


    * **value** (`typing.Any`) – Field’s value.



* **Return type**

    `minos.common.model.fields.Field`



* **Returns**

    A `Field` instance.



#### _property_ name(_: st_ )
Name getter.


* **Return type**

    `str`



#### _property_ parser(_: Optional[Callable[[Any], Any]_ )
Parser getter.


* **Return type**

    `typing.Optional`[`typing.Callable`[[`typing.Any`], `typing.Any`]]



#### _property_ real_type(_: typ_ )
Real Type getter.


* **Return type**

    `type`



#### _property_ type(_: typ_ )
Type getter.


* **Return type**

    `type`



#### _property_ validator(_: Optional[Callable[[Any], Any]_ )
Parser getter.


* **Return type**

    `typing.Optional`[`typing.Callable`[[`typing.Any`], `typing.Any`]]



#### _property_ value(_: An_ )
Value getter.


* **Return type**

    `typing.Any`



### minos.common.model.fields.ModelField()
alias of `minos.common.model.fields.Field`
