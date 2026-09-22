<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Store the number of positive buckets, initially zero:
```
private var distinct = 0

def size: Int = distinct
```
Extend the [representation invariant](../../../../../representation-invariant.md) by

$$
distinct=|\{i:0\leq i<MAX,\ c(i)>0\}|.
$$

The [abstraction function](../../../../../abstraction-function.md) for the [multiset](../../../../../multiset.md) is unchanged. The size operation has no [precondition](../../../../../precondition.md) beyond a valid receiver; it returns the [cardinality](../../../../../cardinality.md) of the [multiset support](../../../../../support-of-a-multiset.md) and changes no state. Replace the modifying methods inside the class by
```
def add(x: Int): Unit = {
  require(inRange(x))
  require(c(x) < Int.MaxValue)
  if (c(x) == 0) distinct += 1
  c(x) += 1
}

def remove(x: Int): Unit = {
  require(inRange(x))
  require(c(x) > 0)
  c(x) -= 1
  if (c(x) == 0) distinct -= 1
}
```
Only transitions from zero to one or from one to zero change the support. [Additions](../../../../../addition.md) to an already positive bucket and removals leaving it positive preserve `distinct`. Thus **`size` takes $O(1)$ time, independently of `MAX`**, and the other operations retain constant-time [array](../../../../../array-data-structure.md) access. Initialization still takes $O(MAX)$ time.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
