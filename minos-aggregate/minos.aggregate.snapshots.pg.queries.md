# minos.aggregate.snapshots.pg.queries module


### _class_ minos.aggregate.snapshots.pg.queries.PostgreSqlSnapshotQueryBuilder(name, condition, ordering=None, limit=None, transaction_uuids=(UUID('00000000-0000-0000-0000-000000000000'),), exclude_deleted=False)
Bases: `object`

PostgreSQL Snapshot Query Builder class.

This class build postgres-compatible database queries over fields based on a condition, ordering, etc.


#### \__init__(name, condition, ordering=None, limit=None, transaction_uuids=(UUID('00000000-0000-0000-0000-000000000000'),), exclude_deleted=False)

#### build()
Build a query.


* **Return type**

    `tuple`[`psycopg2.sql.Composable`, `dict`[`str`, `typing.Any`]]



* **Returns**

    A tuple in which the first value is the sql sentence and the second one is a dictionary containing the
    query parameters.



#### _static_ generate_random_str()
Generate a random string


* **Return type**

    `str`



* **Returns**

    A random string value.
