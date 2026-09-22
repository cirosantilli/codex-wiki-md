<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The diagram omits the type of `carType` and the concrete constructors. Choose `String` selectors `"convertible"`, `"family"`, and `"sports"`, no-argument concrete car constructors, and writable `temperatureScale` and `driverSide` properties on a fresh `Car`. Under this explicit interface convention the two methods are:
```
abstract class Manufacturer {
  def build(carType: String): Car
}

class UKManufacturer extends Manufacturer {
  override def build(carType: String): Car = {
    val car: Car = carType match {
      case "convertible" => new Convertible
      case "family"      => new Family
      case "sports"      => new Sports
      case _ => throw new IllegalArgumentException("Unknown car type: " + carType)
    }
    car.temperatureScale = "Celsius"
    car.driverSide = "left"
    car
  }
}

class USManufacturer extends Manufacturer {
  override def build(carType: String): Car = {
    val car: Car = carType match {
      case "convertible" => new Convertible
      case "family"      => new Family
      case "sports"      => new Sports
      case _ => throw new IllegalArgumentException("Unknown car type: " + carType)
    }
    car.temperatureScale = "Fahrenheit"
    car.driverSide = "right"
    car
  }
}
```
**UK products use Celsius and left-side road traffic; US products use Fahrenheit and right-side road traffic.** Here `driverSide` denotes the side of the road, matching the wording of the source. If the field instead means the side occupied by the steering wheel/driver inside the car, its values must be reversed: right for UK, left for US. The diagram does not resolve that naming ambiguity. With constructor-only immutable properties, pass these same settings to the concrete constructors instead of assigning setters; that is a different interface convention, not a different national policy.

Each branch allocates a fresh concrete `Car`; it does not reuse mutable cars across orders. Invalid selectors fail explicitly rather than returning null. The base price and description come from the chosen concrete product. Options are applied afterward by wrapping the returned car; `build(carType)` has no option-list parameter and therefore cannot infer which options a customer wants.

## ↑ Ancestors (12)

1. [D](../d.md)
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
