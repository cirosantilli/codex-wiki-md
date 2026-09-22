<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [factory method pattern](../../../../../factory-method-pattern.md), `Manufacturer` is the abstract creator and declares `build(carType): Car`; `UKManufacturer` and `USManufacturer` are concrete creators. `Car` is the abstract product interface, and `Convertible`, `Family`, and `Sports` are concrete products. Each national creator selects one product [software class](../../../../../class-programming.md) from `carType` and configures the national settings. The diagram does not contain distinct families of national product interfaces or several abstract product-creation operations, so [abstract factory pattern](../../../../../abstract-factory-pattern.md) is not the most precise identification of this single-operation design.

For the [decorator pattern](../../../../../decorator-pattern.md), `Car` is also the component interface. `Convertible`, `Family`, and `Sports` are concrete components; `Option` is the abstract decorator, both a subtype of `Car` and associated with a wrapped `Car`. `DieselEngine`, `AlarmSystem`, and `AutomaticTransmission` are concrete decorators. Each delegates baseline behavior to its wrapped car, augments `description`, and adds its surcharge to `price`. National properties should delegate unchanged through decorators.

A customer can compose options, for example `new AlarmSystem(new DieselEngine(baseCar))`. Every layer remains usable through the `Car` interface; each layer adds its own description and price contribution. **Factory methods choose/configure the base car, and decorators compose optional additions without requiring a [subclass](../../../../../subclass.md) for every option combination.** If applying each option at most once is required, enforce that as a separate ordering constraint; unrestricted decorator nesting alone permits repeated options.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
