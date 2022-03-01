# minos.aggregate.entities.refs.extractors module


### _class_ minos.aggregate.entities.refs.extractors.RefExtractor(value, type_=None, as_uuids=True)
Bases: `object`

Model Reference Extractor class.


#### \__init__(value, type_=None, as_uuids=True)

#### build()
Run the model reference extractor.


* **Return type**

    `dict`[`str`, `set`[`uuid.UUID`]]



* **Returns**

    A dictionary in which the keys are the class names and the values are the identifiers.
