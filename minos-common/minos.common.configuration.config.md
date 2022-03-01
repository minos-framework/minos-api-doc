# minos.common.configuration.config module


### minos.common.configuration.config.BROKER()
alias of `minos.common.configuration.config.Broker`


### minos.common.configuration.config.DISCOVERY()
alias of `minos.common.configuration.config.Discovery`


### _class_ minos.common.configuration.config.MinosConfig(path, with_environment=True, \*\*kwargs)
Bases: `minos.common.configuration.config.MinosConfigAbstract`

A Minos configuration provides information on the connection points available at that service.
It consists of the following parts:


* Service meta-information (such as name, or version).


* REST Service endpoints available.


* Repository database connection for event sourcing.


* Snapshot database connection.


* Events it publishes/consumes from de given Kafka service.


* Commands it reacts to from other microservices.


* Sagas it takes part on.


#### \__init__(path, with_environment=True, \*\*kwargs)

#### _property_ broker(_: minos.common.configuration.config.Broke_ )
Get the events config.


* **Return type**

    `minos.common.configuration.config.Broker`



* **Returns**

    A `EVENTS` NamedTuple instance.



#### _property_ discovery(_: minos.common.configuration.config.Discover_ )
Get the sagas config.


* **Return type**

    `minos.common.configuration.config.Discovery`



* **Returns**

    A `DISCOVERY` NamedTuple instance.



#### _property_ middleware(_: list[str_ )
Get the commands config.


* **Return type**

    `list`[`str`]



* **Returns**

    A list containing the service class names as string values..



#### _property_ query_repository(_: minos.common.configuration.config.Repositor_ )
Get the query_repository config.


* **Return type**

    `minos.common.configuration.config.Repository`



* **Returns**

    A `QUERY_REPOSITORY` NamedTuple instance.



#### _property_ repository(_: minos.common.configuration.config.Repositor_ )
Get the repository config.


* **Return type**

    `minos.common.configuration.config.Repository`



* **Returns**

    A `REPOSITORY` NamedTuple instance.



#### _property_ rest(_: minos.common.configuration.config.Res_ )
Get the rest config.


* **Return type**

    `minos.common.configuration.config.Rest`



* **Returns**

    A `REST` NamedTuple instance.



#### _property_ saga(_: minos.common.configuration.config.Sag_ )
Get the sagas config.


* **Return type**

    `minos.common.configuration.config.Saga`



* **Returns**

    A `SAGAS` NamedTuple instance.



#### _property_ service(_: minos.common.configuration.config.Servic_ )
Get the service config.


* **Return type**

    `minos.common.configuration.config.Service`



* **Returns**

    A `SERVICE` NamedTuple instance.



#### _property_ services(_: list[str_ )
Get the commands config.


* **Return type**

    `list`[`str`]



* **Returns**

    A list containing the service class names as string values..



#### _property_ snapshot(_: minos.common.configuration.config.Snapsho_ )
Get the snapshot config.


* **Return type**

    `minos.common.configuration.config.Snapshot`



* **Returns**

    A `SNAPSHOT` NamedTuple instance.



### _class_ minos.common.configuration.config.MinosConfigAbstract(path)
Bases: `abc.ABC`

Minos abstract config class.


#### \__init__(path)

### minos.common.configuration.config.QUEUE()
alias of `minos.common.configuration.config.Queue`


### minos.common.configuration.config.REPOSITORY()
alias of `minos.common.configuration.config.Repository`


### minos.common.configuration.config.REST()
alias of `minos.common.configuration.config.Rest`


### minos.common.configuration.config.SAGA()
alias of `minos.common.configuration.config.Saga`


### minos.common.configuration.config.SERVICE()
alias of `minos.common.configuration.config.Service`


### minos.common.configuration.config.SNAPSHOT()
alias of `minos.common.configuration.config.Snapshot`


### minos.common.configuration.config.STORAGE()
alias of `minos.common.configuration.config.Storage`
