# minos.saga.executions.commit module


### _class_ minos.saga.executions.commit.TransactionCommitter(execution_uuid, executed_steps, broker_pool=<dependency_injector.wiring.Provide object>, broker_publisher=<dependency_injector.wiring.Provide object>, \*\*kwargs)
Bases: `object`

Transaction Committer class.


#### \__init__(execution_uuid, executed_steps, broker_pool=<dependency_injector.wiring.Provide object>, broker_publisher=<dependency_injector.wiring.Provide object>, \*\*kwargs)

#### _async_ commit(\*\*kwargs)
Commit the transaction.


* **Parameters**

    **kwargs** – Additional named arguments.



* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### _async_ reject()
Reject the transaction.


* **Return type**

    `None`



* **Returns**

    This method does not return anything.



#### transactions()
Get the list of transactions used during the saga execution.


* **Returns**

    A list of tuples in which the first value is the identifier of the transaction and the second one is
    the name of the microservice in which the saga was executed.
