<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a bounded [linear operator](../../../../../../linear-operator.md) $A:X\to Y$ between [Hilbert spaces](../../../../../../hilbert-space-split.md), let $N=\ker A$ and $R=\operatorname{ran}A$. The [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) is defined on

$$
\mathcal D(A^\dagger)=R\oplus R^\perp.
$$

For $y=Ax+z$, with $z\in R^\perp$, define

$$
\boxed{A^\dagger y=P_{N^\perp}x.}
$$

This is independent of the chosen preimage $x$, since two preimages differ by a vector in $N$. Equivalently, it is the inverse of the restriction of $A$ to $N^\perp$, applied to the component of the data in $R$, and is zero on $R^\perp$.

The generalized solution $x^\dagger=A^\dagger y$ is the unique minimum-norm [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md). Its residual is orthogonal to the range, giving the [operator normal equation](../../../../../../normal-equation-for-a-linear-inverse-problem.md)

$$
\boxed{A^*Ax^\dagger=A^*y,\qquad x^\dagger\in(\ker A)^\perp.}
$$

The [operator normal equation](../../../../../../normal-equation-for-a-linear-inverse-problem.md) alone leaves an arbitrary null-space component; the second condition fixes the minimum-norm representative. The identities $A^\dagger A=P_{N^\perp}$ and $AA^\dagger=P_{\overline R}$ hold on their appropriate domains.

For an infinite-rank [compact operator](../../../../../../compact-operator-split.md), the range need not be closed, and $A^\dagger$ is generally unbounded. Data outside $R\oplus R^\perp$ need not have any [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) at all, even though they can be approximated by range elements. This domain qualification is crucial in part (d); the Moore–Penrose notation does not turn an ill-posed inverse into an everywhere-defined bounded operator.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
