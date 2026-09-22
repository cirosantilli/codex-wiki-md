<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

For a [number field](../../../../../number-field.md) $K$, let $\mathcal O_K$ be its [ring of integers of a number field](../../../../../ring-of-integers.md), $r_1$ the number of real embeddings and $r_2$ the number of conjugate pairs of nonreal complex embeddings, so $[K:\mathbb Q]=r_1+2r_2$. The [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) says

$$
\mathcal O_K^\times\cong\mu(K)\times\mathbb Z^{r_1+r_2-1},
$$

where $\mu(K)$ is the finite group of [roots of unity](../../../../../root-of-unity.md) in $K$. Thus an imaginary [quadratic number field](../../../../../quadratic-field.md) has only roots of unity as units: usually $\{\pm1\}$, with four for $d=-1$ and six for $d=-3$. A real [quadratic number field](../../../../../quadratic-field.md) has units $\pm\epsilon^n$ for a [fundamental unit](../../../../../fundamental-unit-number-theory.md) $\epsilon>1$ and integers $n$.

For $K=\mathbb Q(\sqrt{26})$, $\mathcal O_K=\mathbb Z[\sqrt{26}]$ and the [field norm](../../../../../field-norm.md) is $x^2-26y^2$. The element $\epsilon=5+\sqrt{26}$ has norm $-1$ and is a unit. It is the smallest positive unit greater than one. Indeed for $1<u<\epsilon$, its conjugate is $\pm1/u$, so the coefficient $y=(u\mp1/u)/(2\sqrt{26})$ is a positive integer less than two. Therefore $y=1$, and $x^2=26\pm1$ forces $x=5$, giving $u=\epsilon$, a contradiction. The [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) now gives $\boxed{\mathcal O_K^\times=\{\pm(5+\sqrt{26})^n:n\in\mathbb Z\}}$. Its least positive norm-one generator is $\epsilon^2=51+10\sqrt{26}$.

For the [generalized Pell equation](../../../../../generalized-pell-equation.md), write $\alpha=x+y\sqrt{26}$ with norm $N=\pm10$. Change the sign if necessary and multiply by a power of $\epsilon$ to place it in $\sqrt{10}\leq\alpha<\epsilon\sqrt{10}$. These operations preserve integrality and the absolute norm, though the latter operation can change the norm's sign. Since $\alpha'=N/\alpha$, we have $x=(\alpha+N/\alpha)/2\geq0$ and $y=(\alpha-N/\alpha)/(2\sqrt{26})\geq0$. The upper bound gives $y<4$. Checking $y=0,1,2,3$ in $x^2=26y^2\pm10$ leaves only $(x,y)=(4,1),(6,1)$. Both reduced elements lie in the chosen interval. Therefore **all integral solutions of either sign are**

$$
\boxed{x+y\sqrt{26}=\pm(4+\sqrt{26})(5+\sqrt{26})^n\quad\text{or}\quad\pm(6+\sqrt{26})(5+\sqrt{26})^n,\qquad n\in\mathbb Z.}
$$

Negative powers are integral because $\epsilon^{-1}=\sqrt{26}-5$. In the first family the norm is $-10(-1)^n$ and in the second it is $10(-1)^n$, so this also separates the two equations. The reduction proves exhaustion rather than merely generating examples.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
