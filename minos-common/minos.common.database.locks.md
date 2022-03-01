# minos.common.database.locks module


### _class_ minos.common.database.locks.PostgreSqlLock(wrapped_connection, key, \*args, \*\*kwargs)
Bases: [`minos.common.locks.Lock`](minos.common.locks.md#minos.common.locks.Lock)

“PostgreSql Lock class.


#### \__init__(wrapped_connection, key, \*args, \*\*kwargs)

#### cursor(_: Optional[aiopg.connection.Cursor_ )

#### hashed_key()
Get the hashed key.


* **Returns**

    An integer value.



#### key(_: collections.abc.Hashabl_ )
