<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [monotone decomposition of a submodular set function](../../../../../monotone-decomposition-of-a-submodular-set-function.md) subtracts each element's smallest possible [marginal increment](../../../../../marginal-increment-of-a-set-function.md). For $x\in V$, define

$$
d_x=f(V)-f(V\setminus\{x\}),\qquad
h(S)=f(\varnothing)+\sum_{x\in S}d_x,\qquad
g(S)=f(S)-h(S).
$$

The [set function](../../../../../set-function.md) $h$ is a [modular set function](../../../../../modular-set-function.md): the contributions of each element, and the constant $f(\varnothing)$, cancel in

$$
h(A)+h(B)=h(A\cap B)+h(A\cup B).
$$

Subtracting this equality from the [submodularity](../../../../../submodular-set-function.md) inequality for $f$ proves that $g$ is a [submodular set function](../../../../../submodular-set-function.md). Also $g(\varnothing)=0$, so it is a [normalised set function](../../../../../normalised-set-function.md).

For $x\notin S$, the inclusion $S\subseteq V\setminus\{x\}$ and [diminishing returns](../../../../../diminishing-returns-characterization-of-submodularity.md) imply

$$
\Delta_x g(S)=\Delta_x f(S)-d_x\geq0.
$$

Adding elements one at a time now proves that $g$ is a [monotone set function](../../../../../monotone-set-function.md). Since it starts at zero, it is also a [nonnegative function](../../../../../nonnegative-function.md). Thus **$f=g+h$ has all the required properties**.

Here [modular set function](../../../../../modular-set-function.md) means equality in the intersection–union identity; a constant term is allowed. If one imposed the additional convention $h(\varnothing)=0$, the claimed decomposition of an arbitrary $f$ would require $f(\varnothing)=0$. The displayed constant is essential for the problem as stated. For $V=\varnothing$, take $g=0$ and $h=f$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Combinatorial optimisation](../../../combinatorial-optimisation-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
