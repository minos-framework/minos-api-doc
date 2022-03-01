# minos.aggregate.exceptions module


### _exception_ minos.aggregate.exceptions.AggregateException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base Aggregate module exception


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.AlreadyDeletedException(error_message)
Bases: `minos.aggregate.exceptions.SnapshotRepositoryException`

Exception to be raised when a `RootEntity` is already deleted from the repository.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.EventRepositoryConflictException(error_message, offset)
Bases: `minos.aggregate.exceptions.EventRepositoryException`

Exception to be raised when some `EventEntry` raises a conflict.


#### \__init__(error_message, offset)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.EventRepositoryException(error_message)
Bases: `minos.aggregate.exceptions.AggregateException`

Base event repository exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.NotFoundException(error_message)
Bases: `minos.aggregate.exceptions.SnapshotRepositoryException`

Exception to be raised when a `RootEntity` is not found on the repository.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.SnapshotRepositoryConflictException(previous, event)
Bases: `minos.aggregate.exceptions.SnapshotRepositoryException`

Exception to be raised when current version is newer than the one to be processed.


#### \__init__(previous, event)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.SnapshotRepositoryException(error_message)
Bases: `minos.aggregate.exceptions.AggregateException`

Base snapshot exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.TransactionNotFoundException(error_message)
Bases: `minos.aggregate.exceptions.TransactionRepositoryException`

Exception to be raised when some transaction is not found on the repository.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.TransactionRepositoryConflictException(error_message)
Bases: `minos.aggregate.exceptions.TransactionRepositoryException`

Exception to be raised when a transactions has invalid status.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.TransactionRepositoryException(error_message)
Bases: `minos.aggregate.exceptions.AggregateException`

Base transaction repository exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.aggregate.exceptions.ValueObjectException(error_message)
Bases: `minos.aggregate.exceptions.AggregateException`

If an attribute of an immutable class is modified, this exception will be raised


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.
