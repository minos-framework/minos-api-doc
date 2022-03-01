# minos.common.exceptions module


### _exception_ minos.common.exceptions.DataDecoderException(error_message)
Bases: `minos.common.exceptions.MinosModelException`

Base data decoder exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.DataDecoderMalformedTypeException(error_message)
Bases: `minos.common.exceptions.DataDecoderException`

Exception to be raised when malformed types are provided.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.DataDecoderRequiredValueException(error_message)
Bases: `minos.common.exceptions.DataDecoderException`

Exception to be raised when required values are not provided.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.DataDecoderTypeException(target_type, value)
Bases: `minos.common.exceptions.DataDecoderException`

Exception to be raised when expected and provided types do not match.


#### \__init__(target_type, value)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.EmptyMinosModelSequenceException(error_message)
Bases: `minos.common.exceptions.MinosModelException`

Exception to be raised when a sequence must be not empty, but it is empty.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosAttributeValidationException(name, value)
Bases: `minos.common.exceptions.MinosModelAttributeException`

Exception to be raised when some fields are not valid.


#### \__init__(name, value)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosBrokerException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base broker exception


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosConfigException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base config exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosException(error_message)
Bases: `Exception`

Exception class for import packages or modules


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosHandlerException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base handler exception


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosImportException(error_message)
Bases: `minos.common.exceptions.MinosException`


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosLockException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base lock exception


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosMalformedAttributeException(error_message)
Bases: `minos.common.exceptions.MinosModelAttributeException`

Exception to be raised when there are any kind of problems with the type definition.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosMessageException(error_message)
Bases: `minos.common.exceptions.MinosException`


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosModelAttributeException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base model attributes exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosModelException(error_message)
Bases: `minos.common.exceptions.MinosException`

Exception to be raised when some mandatory condition is not satisfied by a model.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosParseAttributeException(name, value, exception)
Bases: `minos.common.exceptions.MinosModelAttributeException`

Exception to be raised when there are any kind of problems with the parsing logic.


#### \__init__(name, value, exception)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosProtocolException(error_message)
Bases: `minos.common.exceptions.MinosException`


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosReqAttributeException(error_message)
Bases: `minos.common.exceptions.MinosModelAttributeException`

Exception to be raised when some required attributes are not provided.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MinosTypeAttributeException(name, target_type, value)
Bases: `minos.common.exceptions.MinosModelAttributeException`

Exception to be raised when there are any mismatching between the expected and observed attribute type.


#### \__init__(name, target_type, value)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.MultiTypeMinosModelSequenceException(error_message)
Bases: `minos.common.exceptions.MinosModelException`

Exception to be raised when a sequence doesn’t satisfy the condition to have the same type for each item.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.common.exceptions.NotProvidedException(error_message)
Bases: `minos.common.exceptions.MinosException`

Exception to be raised when a dependency is needed but not provided.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.
