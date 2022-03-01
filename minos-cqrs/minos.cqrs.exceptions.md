# minos.cqrs.exceptions module


### _exception_ minos.cqrs.exceptions.MinosCqrsException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base CQRS exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.cqrs.exceptions.MinosIllegalHandlingException(error_message)
Bases: `minos.common.exceptions.MinosException`

Exception to be raised when a service is trying to be used to handle improper message types.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.cqrs.exceptions.MinosNotAnyMissingReferenceException(error_message)
Bases: `minos.cqrs.exceptions.MinosQueryServiceException`

Exception to be raised when an aggregate diff does not have any missing reference.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.cqrs.exceptions.MinosQueryServiceException(error_message)
Bases: `minos.cqrs.exceptions.MinosCqrsException`

Exception to be raised by query service when an internal error is raised.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.
