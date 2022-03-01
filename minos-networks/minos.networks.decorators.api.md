# minos.networks.decorators.api module


### _class_ minos.networks.decorators.api.BrokerEnroute()
Bases: `object`

Broker Enroute class


#### command()
alias of [`minos.networks.decorators.definitions.broker.BrokerCommandEnrouteDecorator`](minos.networks.decorators.definitions.broker.md#minos.networks.decorators.definitions.broker.BrokerCommandEnrouteDecorator)


#### event()
alias of [`minos.networks.decorators.definitions.broker.BrokerEventEnrouteDecorator`](minos.networks.decorators.definitions.broker.md#minos.networks.decorators.definitions.broker.BrokerEventEnrouteDecorator)


#### query()
alias of [`minos.networks.decorators.definitions.broker.BrokerQueryEnrouteDecorator`](minos.networks.decorators.definitions.broker.md#minos.networks.decorators.definitions.broker.BrokerQueryEnrouteDecorator)


### _class_ minos.networks.decorators.api.Enroute()
Bases: `object`

Enroute decorator main class


#### broker()
alias of `minos.networks.decorators.api.BrokerEnroute`


#### periodic()
alias of `minos.networks.decorators.api.PeriodicEnroute`


#### rest()
alias of `minos.networks.decorators.api.RestEnroute`


### _class_ minos.networks.decorators.api.PeriodicEnroute()
Bases: `object`

Periodic Enroute class.


#### event()
alias of [`minos.networks.decorators.definitions.periodic.PeriodicEventEnrouteDecorator`](minos.networks.decorators.definitions.periodic.md#minos.networks.decorators.definitions.periodic.PeriodicEventEnrouteDecorator)


### _class_ minos.networks.decorators.api.RestEnroute()
Bases: `object`

Rest Enroute class


#### command()
alias of [`minos.networks.decorators.definitions.rest.RestCommandEnrouteDecorator`](minos.networks.decorators.definitions.rest.md#minos.networks.decorators.definitions.rest.RestCommandEnrouteDecorator)


#### query()
alias of [`minos.networks.decorators.definitions.rest.RestQueryEnrouteDecorator`](minos.networks.decorators.definitions.rest.md#minos.networks.decorators.definitions.rest.RestQueryEnrouteDecorator)


### minos.networks.decorators.api.enroute()
alias of `minos.networks.decorators.api.Enroute`
