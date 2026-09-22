<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [immutable object](../../../../../immutable-object.md) has no changeable observable state after its [object constructor](../../../../../object-constructor.md) finishes. Two clients may hold references to the same [immutable object](../../../../../immutable-object.md), but neither can change what the other observes. Thus sharing an [immutable object](../../../../../immutable-object.md) avoids the interference normally associated with [reference aliasing](../../../../../reference-aliasing.md): for example, sharing a [Java](../../../../../java-programming-language.md) `String` is safe because a text-changing operation returns another [software object](../../../../../software-object.md) rather than modifying that [String data type](../../../../../string-data-type.md) value.

A `final` reference alone does not establish an [immutable object](../../../../../immutable-object.md): it prevents reassignment of that reference, but its referent could still be mutable. An [immutable object](../../../../../immutable-object.md) must also protect any reachable mutable state, for instance through [defensive copying](../../../../../defensive-copying.md). With that qualification, the essential answer is

$$
\boxed{\text{unchanging observable state permits sharing without update interference}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
