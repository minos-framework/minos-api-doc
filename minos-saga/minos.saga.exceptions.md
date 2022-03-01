# minos.saga.exceptions module


### _exception_ minos.saga.exceptions.AlreadyCommittedException(error_message)
Bases: `minos.saga.exceptions.SagaException`

Exception to be raised when trying to modifying an already committed saga.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.AlreadyOnSagaException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when a saga step is already in another saga.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.EmptySagaException(message=None)
Bases: `minos.saga.exceptions.SagaException`

Exception to be raised when saga is empty.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.EmptySagaStepException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when the step is empty.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.ExecutorException(exception, message=None)
Bases: `minos.saga.exceptions.SagaException`

Exception to be raised when a saga executor raises some exception.


#### \__init__(exception, message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.MultipleElseThenException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when multiple else then alternatives are defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.MultipleOnErrorException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when multiple on error methods are defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.MultipleOnExecuteException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when multiple on execute methods are defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.MultipleOnFailureException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when multiple on failure methods are defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.MultipleOnSuccessException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when multiple on success methods are defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base saga exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaExecutionAlreadyExecutedException(error_message)
Bases: `minos.saga.exceptions.SagaExecutionException`

Exception to be raised when a saga execution cannot be executed.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaExecutionException(error_message)
Bases: `minos.saga.exceptions.SagaException`

Base exception for saga execution.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaExecutionNotFoundException(error_message)
Bases: `minos.saga.exceptions.SagaExecutionException`

Exception to be raised when a saga execution is not found.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaFailedCommitCallbackException(exception, message=None)
Bases: `minos.saga.exceptions.SagaFailedExecutionException`

Exception to be raised when a saga commit callback raises some exception


#### \__init__(exception, message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaFailedExecutionException(exception, message=None)
Bases: `minos.saga.exceptions.SagaExecutionException`

Exception to be raised when a saga execution failed while running.


#### \__init__(exception, message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaFailedExecutionStepException(exception, message=None)
Bases: `minos.saga.exceptions.SagaStepExecutionException`, `minos.saga.exceptions.SagaFailedExecutionException`

Exception to be raised when a saga execution step failed while running.


#### \__init__(exception, message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaNotCommittedException(message=None)
Bases: `minos.saga.exceptions.SagaException`

Exception to be raised when trying to exec a  not committed saga.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaNotDefinedException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when the saga is not defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaPausedExecutionStepException(message=None)
Bases: `minos.saga.exceptions.SagaStepExecutionException`

Exception to be raised when a saga execution step is paused.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaResponseException(error_message)
Bases: `minos.saga.exceptions.SagaException`

Exception to be used when `CommandStatus` is not `SUCCESS`


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaRollbackExecutionException(error_message)
Bases: `minos.saga.exceptions.SagaExecutionException`

Exception to be raised when a saga exception cannot be rollbacked


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaRollbackExecutionStepException(error_message)
Bases: `minos.saga.exceptions.SagaStepExecutionException`

Exception to be raised when a saga execution step failed while performing a rollback.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaStepException(error_message)
Bases: `minos.saga.exceptions.SagaException`

Base exception for saga steps.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.SagaStepExecutionException(error_message)
Bases: `minos.saga.exceptions.SagaException`

Base exception for saga execution step.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.saga.exceptions.UndefinedOnExecuteException(message=None)
Bases: `minos.saga.exceptions.SagaStepException`

Exception to be raised when the on execute method is not defined.


#### \__init__(message=None)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.
