# minos.networks.exceptions module


### _exception_ minos.networks.exceptions.MinosActionNotFoundException(error_message)
Bases: `minos.networks.exceptions.MinosHandlerException`

Exception to be raised when an action cannot be found,


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosDiscoveryConnectorException(error_message)
Bases: `minos.networks.exceptions.MinosNetworkException`

Exception to be raised when there is a failure while communicating with the discovery.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosEnrouteDecoratorException(error_message)
Bases: `minos.networks.exceptions.MinosNetworkException`

Base exception for enroute decorators.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosHandlerException(error_message)
Bases: `minos.networks.exceptions.MinosNetworkException`

Base handler exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosHandlerNotFoundEnoughEntriesException(error_message)
Bases: `minos.networks.exceptions.MinosHandlerException`

Exception to be raised when not enough entries have been found by a handler.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosInvalidDiscoveryClient(error_message)
Bases: `minos.networks.exceptions.MinosNetworkException`

Exception raised when the configured Discovery Client does not implement de DiscoveryClient interface


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosMultipleEnrouteDecoratorKindsException(error_message)
Bases: `minos.networks.exceptions.MinosEnrouteDecoratorException`

Exception to be raised when multiple enroute decorator kinds are applied to the same function.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosNetworkException(error_message)
Bases: `minos.common.exceptions.MinosException`

Base network exception.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.MinosRedefinedEnrouteDecoratorException(error_message)
Bases: `minos.networks.exceptions.MinosEnrouteDecoratorException`

Exception to be raised when same enroute decorator is used by multiple actions.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.NotHasContentException(error_message)
Bases: `minos.networks.exceptions.RequestException`

Exception to be raised when request has not content.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.NotHasParamsException(error_message)
Bases: `minos.networks.exceptions.RequestException`

Exception to be raised when request has not params.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.NotSatisfiedCheckerException(error_message)
Bases: `minos.networks.exceptions.MinosHandlerException`

Exception to be raised when some checkers are not validated.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.


### _exception_ minos.networks.exceptions.RequestException(error_message)
Bases: `minos.networks.exceptions.MinosNetworkException`

Base exception for requests.


#### \__init__(error_message)

#### args()

#### with_traceback()
Exception.with_traceback(tb) –
set self.__traceback__ to tb and return self.
