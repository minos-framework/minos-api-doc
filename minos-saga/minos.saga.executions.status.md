# minos.saga.executions.status module


### _class_ minos.saga.executions.status.SagaStatus(value)
Bases: `enum.Enum`

Saga Status class.


#### Created(_ = 'created_ )

#### Errored(_ = 'errored_ )

#### Finished(_ = 'finished_ )

#### Paused(_ = 'paused_ )

#### Running(_ = 'running_ )

#### _classmethod_ from_raw(raw)
Build a new instance from raw.


* **Parameters**

    **raw** (`typing.Union`[`str`, `minos.saga.executions.status.SagaStatus`]) – The raw representation of the instance.



* **Return type**

    `minos.saga.executions.status.SagaStatus`



* **Returns**

    A `SagaStatus` instance.



#### _property_ raw(_: st_ )
Compute the raw representation of the instance.


* **Return type**

    `str`



* **Returns**

    A `str` instance.



### _class_ minos.saga.executions.status.SagaStepStatus(value)
Bases: `enum.Enum`

Saga Step Status class.


#### Created(_ = 'created_ )

#### ErroredByOnExecute(_ = 'errored-by-on-execute_ )

#### ErroredOnError(_ = 'errored-on-error_ )

#### ErroredOnExecute(_ = 'errored-on-execute_ )

#### ErroredOnFailure(_ = 'errored-on-failure_ )

#### ErroredOnSuccess(_ = 'errored-on-success_ )

#### Finished(_ = 'finished_ )

#### FinishedOnExecute(_ = 'finished-on-execute_ )

#### PausedByOnExecute(_ = 'paused-by-on-execute_ )

#### PausedOnFailure(_ = 'paused-on-failure_ )

#### RunningOnError(_ = 'running-on-error_ )

#### RunningOnExecute(_ = 'running-on-execute_ )

#### RunningOnFailure(_ = 'running-on-failure_ )

#### RunningOnSuccess(_ = 'running-on-success_ )

#### _classmethod_ from_raw(raw)
Build a new instance from raw.


* **Parameters**

    **raw** (`typing.Union`[`str`, `minos.saga.executions.status.SagaStepStatus`]) – The raw representation of the instance.



* **Return type**

    `minos.saga.executions.status.SagaStepStatus`



* **Returns**

    A `SagaStepStatus` instance.



#### _property_ raw(_: st_ )
Compute the raw representation of the instance.


* **Return type**

    `str`



* **Returns**

    A `str` instance.
