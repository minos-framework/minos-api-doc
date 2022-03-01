# minos.saga.definitions.steps.abc module


### _class_ minos.saga.definitions.steps.abc.SagaStep(saga=None, \*\*kwargs)
Bases: `abc.ABC`

Saga step class.


#### \__init__(saga=None, \*\*kwargs)

#### commit(\*args, \*\*kwargs)
Commit the current `SagaStep` on the `Saga`.


* **Parameters**

    
    * **args** – Additional positional arguments.


    * **kwargs** – Additional named arguments.



* **Return type**

    [`minos.saga.definitions.saga.Saga`](minos.saga.definitions.saga.md#minos.saga.definitions.saga.Saga)



* **Returns**

    A `Saga` instance.



#### conditional_step(\*args, \*\*kwargs)
Create a new conditional step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.conditional.ConditionalSagaStep`](minos.saga.definitions.steps.conditional.md#minos.saga.definitions.steps.conditional.ConditionalSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### _classmethod_ from_raw(raw, \*\*kwargs)
Build a new instance from raw.


* **Parameters**

    
    * **raw** (`typing.Union`[`dict`[`str`, `typing.Any`], `minos.saga.definitions.steps.abc.SagaStep`]) – A raw representation.


    * **kwargs** – Additional named arguments.



* **Return type**

    `minos.saga.definitions.steps.abc.SagaStep`



* **Returns**

    A `SagaStep` instance.



#### local_step(\*args, \*\*kwargs)
Create a new local step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.local.LocalSagaStep`](minos.saga.definitions.steps.local.md#minos.saga.definitions.steps.local.LocalSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### _abstract property_ raw(_: dict[str, Any_ )
Generate a raw representation of the instance.


* **Return type**

    `dict`[`str`, `typing.Any`]



* **Returns**

    A `dict` instance.



#### remote_step(\*args, \*\*kwargs)
Create a new remote step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    [`minos.saga.definitions.steps.remote.RemoteSagaStep`](minos.saga.definitions.steps.remote.md#minos.saga.definitions.steps.remote.RemoteSagaStep)



* **Returns**

    A new `SagaStep` instance.



#### step(\*args, \*\*kwargs)
Create a new step in the `Saga`.


* **Parameters**

    
    * **args** – Additional positional parameters.


    * **kwargs** – Additional named parameters.



* **Return type**

    `minos.saga.definitions.steps.abc.SagaStep`



* **Returns**

    A new `SagaStep` instance.



#### _abstract_ validate()
Check if the step is valid.


* **Return type**

    `None`



* **Returns**

    This method does not return anything, but raises an exception if the step is not valid.
