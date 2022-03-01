# minos.networks.rest.services module


### _class_ minos.networks.rest.services.RestService(\*\*kwargs)
Bases: `aiomisc.service.aiohttp.AIOHTTPService`

Rest Interface

Expose REST Interface handler using aiomisc AIOHTTPService.


#### \__init__(\*\*kwargs)

#### _property_ context(_: aiomisc.context.Contex_ )

* **Return type**

    `aiomisc.context.Context`



#### _async_ create_application()
Create the web application.


* **Return type**

    `aiohttp.web_app.Application`



* **Returns**

    A `web.Application` instance.



#### _async_ create_site()

* **Return type**

    `aiohttp.web_runner.SockSite`



#### runner(_: aiohttp.web_runner.BaseRunne_ )

#### set_loop(loop)

* **Return type**

    `None`



#### site(_: aiohttp.web_runner.SockSit_ )

#### _async_ start()

* **Return type**

    `None`



#### _property_ start_event(_: asyncio.locks.Even_ )

* **Return type**

    `asyncio.locks.Event`



#### _async_ stop(exception=None)

* **Return type**

    `None`
