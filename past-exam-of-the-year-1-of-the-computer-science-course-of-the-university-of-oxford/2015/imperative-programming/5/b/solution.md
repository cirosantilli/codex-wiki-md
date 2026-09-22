<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write each [Scala trait linearization](../../../../../scala-trait-linearization.md) from most specific to least specific. Merge the parents' [Scala trait linearizations](../../../../../scala-trait-linearization.md) right-to-left, removing a duplicate from the earlier portion when it also appears in the later portion. This retains every base once while respecting its required position after derived [traits](../../../../../trait.md).[Class Linearization](../../../../../scala-2-11-classes-and-objects-specification.md)
```
CityMan, City, Earth, Man, Mammal, Animal, Describe

BirdMan, City, Earth, Man, Mammal, Bird, Animal, Describe

BatMan, Man, Gotham, City, US, Earth, Bat, Mammal, Bird, Animal, Describe
```
For example, combining the final `City` with `Gotham` does not put `City` before its derived [trait](../../../../../trait.md) `Gotham`; duplicate removal places it after `Gotham`. Similarly `Mammal` and `Bird` remain after `Bat`, despite their occurrence through other parents.

Each `describe` calls `super.describe` before appending its own label. Thus execution enters implementations along the displayed [Scala trait linearization](../../../../../scala-trait-linearization.md), and appends labels in reverse order when calls return. The three printed lines are
```
Describe, Animal, Mammal, Man, Earth, City, 
Describe, Animal, Bird, Mammal, Man, Earth, City, 
Describe, Animal, Bird, Mammal, Bat, Earth, US, City, Gotham, Man, 
```
Each line has a final comma and space, because every printed [string](../../../../../string.md) fragment includes them. The essential result is

$$
\boxed{\text{Output labels follow the reverse linearization, excluding the concrete class.}}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
