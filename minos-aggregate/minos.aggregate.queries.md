# minos.aggregate.queries module

minos.common.queries module.


### _class_ minos.aggregate.queries.Condition()
Bases: `object`

Condition class.

This class provides the way to create filtering conditions for `Model` instances based on the following operators:


* TRUE: Always evaluates as True.


* FALSE: Always evaluates as True.


* AND: Only evaluates as True if all the given conditions are evaluated as True.


* OR: Evaluates as True if at least one of the given conditions are evaluated as True.


* NOT: Evaluates as True only if the inner condition is evaluated as False.


* LOWER: Evaluates as True only if the field of the given model is lower (<) than the parameter.


* LOWER_EQUAL: Evaluates as True only if the field of the given model is lower or equal (<=) to the parameter.


* GREATER: Evaluates as True only if the field of the given model is greater (>) than the parameter.


* GREATER_EQUAL: Evaluates as True only if the field of the given model is greater or equal (>=) to the

parameter.
\* EQUAL: Evaluates as True only if the field of the given model is equal (==) to the parameter.
\* NOT_EQUAL: Evaluates as True only if the field of the given model is not equal (!=) to the parameter.
\* IN: Evaluates as True only if the field of the given model belongs (in) to the parameter (which must be a
collection).
\* LIKE: Evaluates as True only if the field of the given model matches to the parameter _pattern.

For example, to define a condition in which the year must be between 1994 and 2003 or the color must be
blue, the condition can be writen as:

```default
Condition.OR(
    Condition.AND(Condition.GREATER_EQUAL("year", 1994), Condition.LOWER("year", 2003)),
    Condition.EQUAL("color", "blue")
)
```


#### AND()
alias of `minos.aggregate.queries._AndCondition`


#### EQUAL()
alias of `minos.aggregate.queries._EqualCondition`


#### FALSE(_ = _FalseCondition(_ )

#### GREATER()
alias of `minos.aggregate.queries._GreaterCondition`


#### GREATER_EQUAL()
alias of `minos.aggregate.queries._GreaterEqualCondition`


#### IN()
alias of `minos.aggregate.queries._InCondition`


#### LIKE()
alias of `minos.aggregate.queries._LikeCondition`


#### LOWER()
alias of `minos.aggregate.queries._LowerCondition`


#### LOWER_EQUAL()
alias of `minos.aggregate.queries._LowerEqualCondition`


#### NOT()
alias of `minos.aggregate.queries._NotCondition`


#### NOT_EQUAL()
alias of `minos.aggregate.queries._NotEqualCondition`


#### OR()
alias of `minos.aggregate.queries._OrCondition`


#### TRUE(_ = _TrueCondition(_ )

### _class_ minos.aggregate.queries.Ordering()
Bases: `object`

Ordering class.

This class provides the way to define ordering strategies for `Model` instances through the `ASC` and `DESC`
class methods, which retrieves instances containing the given information.

For example, to define a descending ordering strategy by the name field:

```default
Ordering.DESC("name")
```


#### ASC(_ = functools.partial(<class 'minos.aggregate.queries._Ordering'>, reverse=False_ )

#### DESC(_ = functools.partial(<class 'minos.aggregate.queries._Ordering'>, reverse=True_ )
