<h1 id="a/1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First take the usual positive-parameter limit $\epsilon\downarrow0$. For real $x$, the equation implies $|x^2-1|\leq\epsilon$, so every root lies near $1$ or $-1$. Near the positive root,

$$
\tanh(x/\epsilon)=1+O(e^{-2x/\epsilon}),
$$

and hence $x^2=1-\epsilon$ up to an exponentially small correction. Near the negative root, the corresponding limit is minus one, giving $x^2=1+\epsilon$ to all algebraic orders. Expanding the square roots gives

$$
\boxed{x_+=1-\frac{\epsilon}{2}+O(\epsilon^2),
\qquad x_-=-1-\frac{\epsilon}{2}+O(\epsilon^2).}
$$

There is one root in each neighborhood: the [derivative](../../../../../derivative.md) $2x+\operatorname{sech}^2(x/\epsilon)$ has the sign of $x$ there for sufficiently small positive $\epsilon$. The bound above excludes further real roots.

If the source's unqualified $\epsilon\to0$ is read as a two-sided limit, use the exact identity

$$
\epsilon\tanh(x/\epsilon)
=|\epsilon|\tanh(x/|\epsilon|).
$$

The two-sided versions therefore replace $\epsilon$ by $|\epsilon|$ in both displayed first corrections. The two one-sided algebraic expansions otherwise have the same reasoning.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
