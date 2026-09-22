<h1 id="12f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $g(n,k)=r(n)$, where $r$ is the total primitive-recursive parity function from part (ii), and apply [unbounded minimization](../../../../../../mu-operator.md) in $k$:

$$
p(n)=\mu k\,[g(n,k)=0].
$$

If $n$ is even, then $g(n,0)=0$ and $p(n)=0$. If $n$ is odd, then $g(n,k)=1$ for every $k$, so the search never terminates and $p(n)$ is undefined. Hence $p$ is partial recursive. Because every function built without minimization is total, $p$ cannot be defined without minimization; the functions $s$ and $r$ can.

It remains to characterize the functions built using only the initial functions and composition. They are exactly the [functions](../../../../../../composition-only-recursive-function.md)

$$
\boxed{f(x_1,\ldots,x_k)=c
\quad\hbox{or}\quad
f(x_1,\ldots,x_k)=x_i+c}
$$

for some $c\in\mathbb N$ and some input coordinate $i$.

Indeed, the [zero function](../../../../../../zero-function.md) is the first form, the [successor function](../../../../../../successor-function.md) and each [projection function](../../../../../../projection-function.md) have the second form, and composing functions of these forms preserves the classification: a constant outer function remains constant, while an outer function $y_j+c$ selects one inner function and adds $c$. This proves necessity by [structural induction](../../../../../../structural-induction.md). Conversely, applying the successor function $c$ times to zero produces the constant $c$, and applying it $c$ times to $\pi_i^k$ produces $x_i+c$.

Every function in this class is directly [computable](../../../../../../total-computable-function.md): an algorithm either writes the fixed constant $c$, or copies the $i$th input and performs $c$ successor steps.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
