<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A fixed-size [array](../../../../../array-data-structure.md) cannot implement unbounded successful insertion. **Either specify a bounded [double-ended queue](../../../../../double-ended-queue.md) with an extra not-full insertion [precondition](../../../../../precondition.md), or retain the unbounded interface and specify a possible full-capacity failure.** Silently overwriting an endpoint would change the stated behavior. Here use the bounded contract, with a fixed positive capacity `MAX` and abstract state $|s|\leq MAX$. Both additions require $|s|<MAX$; the other [postconditions](../../../../../postcondition.md) remain unchanged. The class declaration in part (c) is interpreted as implementing this explicitly revised contract, rather than as a behavioral subtype of the unrestricted contract in part (a).

The concrete state is an [array](../../../../../array-data-structure.md) `a` of length `MAX`, a first-position index `head`, and an occupied-entry count `size`. Its [representation invariant](../../../../../representation-invariant.md) is

$$
MAX>0,\qquad a.length=MAX,\qquad 0\leq head<MAX,\qquad0\leq size\leq MAX.
$$

The [abstraction function](../../../../../abstraction-function.md) is $s(k)=a((head+k)\bmod MAX)$ for $0\leq k<size$. Unoccupied slots are unconstrained. Storing `size` distinguishes empty and full states even though their two circular endpoint positions coincide. `MAX=1` is valid. Using a [circular buffer](../../../../../circular-buffer.md) avoids shifting entries and makes every endpoint operation [constant time](../../../../../constant-time.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
