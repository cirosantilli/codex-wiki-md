<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [string data type](../../../../string-data-type.md) suffices for a name, an [algebraic data type](../../../../algebraic-data-type.md) for the recorded sex, and a triple of [integers](../../../../integer-split.md) for a date. Use a constructor for `Person` so that selectors are unambiguous in [Haskell](../../../../haskell.md):

```
type Name = String
data Sex = Female | Male deriving (Eq, Show)
data Date = Date { day :: Int, month :: Int, year :: Int }
  deriving (Eq, Show)
data Person = Person { name :: Name, sex :: Sex, born :: Date }
  deriving (Eq, Show)
type BirthCertificate = (Person, Person, Person)
type Database = [BirthCertificate]
```

Dates have the [precondition](../../../../precondition.md) that their fields form a valid calendar date. This simple [database](../../../../database.md) representation assumes the triple of identifying fields distinguishes the recorded individuals; a production [database](../../../../database.md) would normally add a stable identifier to distinguish namesakes. The two constructors for `Sex` model the two recorded values used by this exercise. In mathematical notation,

$$
\boxed{\mathrm{Person}=\mathrm{Name}\times\mathrm{Sex}\times\mathrm{Date}.}
$$

## ↑ Ancestors (11)

1. [3](../3.md)
2. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
3. [2003](../../split.md)
4. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../split.md)
5. [Year 1 of the computer science course of the University of Oxford](../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
6. [Computer science course of the University of Oxford](../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
