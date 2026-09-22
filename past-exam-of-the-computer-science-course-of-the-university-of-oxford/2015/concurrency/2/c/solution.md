<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $f$ is [injective](../../../../../injective-function.md), the equation is true:

$$
\boxed{f(P\underset A\Vert Q)=f(P)\underset{f(A)}\Vert f(Q)\qquad(f\text{ injective}).}
$$

For a [CSP event](../../../../../csp-event.md) $a\in A$, the original [CSP parallel composition](../../../../../csp-parallel-composition.md) permits $a$ exactly when both operands can perform $a$. After [CSP event renaming](../../../../../csp-event-renaming.md), the corresponding rule requires the same image $f(a)$ in both operands. [Injectivity](../../../../../injective-function.md) ensures that matching images came from the same event, and that an event outside $A$ cannot acquire the image of one inside $A$. Independent transitions remain independent, and [CSP internal actions](../../../../../csp-internal-action.md) are unchanged. Matching these transition rules gives a [strong bisimulation](../../../../../strong-bisimulation.md), hence equality in all three standard [CSP semantic models](../../../../../csp-semantic-model.md).

For a non-injective $f$, the equation need not hold. Let

$$
P=a\to\mathrm{STOP},\quad Q=b\to\mathrm{STOP},\quad A=\{a,b\},\quad a\ne b,\quad f(a)=f(b)=c.
$$

On the left, both events require [synchronization](../../../../../synchronization-computing.md) but the other operand offers the wrong event, so $P\underset A\Vert Q=\mathrm{STOP}$. On the right, both renamed operands offer $c$, which can synchronize:

$$
\boxed{f(P\underset A\Vert Q)=\mathrm{STOP}\ne c\to\mathrm{STOP}=f(P)\underset{f(A)}\Vert f(Q).}
$$

The failure is already visible in the [CSP traces model](../../../../../csp-traces-model.md). A particular non-injective [CSP event renaming](../../../../../csp-event-renaming.md) may still preserve a particular composition; it is the unrestricted equivalence that fails.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
