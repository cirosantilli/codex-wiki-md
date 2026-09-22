<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [relational schema](../../../../../relational-schema.md) and [functional dependency](../../../../../functional-dependency.md)

$$
\boxed{R(b,a),\qquad F=\{b\to a\}.}
$$

The [attribute closure](../../../../../attribute-closure.md) of $\{b\}$ is $\{b,a\}$, so $\{b\}$ is a [candidate key](../../../../../candidate-key.md). The [attribute closure](../../../../../attribute-closure.md) of $\{a\}$ is just $\{a\}$, so it is not a [superkey](../../../../../superkey.md). The set $\{a,b\}$ is a [superkey](../../../../../superkey.md) but is not a [candidate key](../../../../../candidate-key.md), because removing $a$ leaves the [superkey](../../../../../superkey.md) $\{b\}$. Thus the only [candidate key](../../../../../candidate-key.md) is $\{b\}$, and $a$ occurs in none.

For example, records $(b,a)=(1,7),(2,7)$ illustrate that the same $a$ value may occur at different $b$ values. The conclusion about [candidate keys](../../../../../candidate-key.md) follows from the declared [functional dependencies](../../../../../functional-dependency.md), rather than from accidental uniqueness in any one sample.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
