<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the Hausdorff convention for a [locally convex space](../../../../../locally-convex-space.md): a real vector space $X$ is equipped with a separating family $\mathcal P$ of [seminorms](../../../../../seminorm.md). Thus each $p$ is nonnegative, subadditive and satisfies $p(tx)=|t|p(x)$, and for every $x\neq0$ some $p\in\mathcal P$ has $p(x)>0$. The topology has a neighborhood basis at $a\in X$ consisting of

$$
a+\{x:p_1(x)<\varepsilon_1,\ldots,p_m(x)<\varepsilon_m\},\qquad p_i\in\mathcal P,\quad\varepsilon_i>0.
$$

Equivalently, it is the coarsest vector-space topology making all these [seminorms](../../../../../seminorm.md) continuous. The separating condition is precisely what makes this topology Hausdorff. If the Hausdorff requirement were omitted, continuous [linear functionals](../../../../../linear-functional.md) could not distinguish points in the common kernel of the [seminorms](../../../../../seminorm.md).

The [continuous dual space](../../../../../continuous-dual-space-split.md) $X^*$ consists of all [continuous linear functionals](../../../../../continuous-linear-functional.md) $X\to\mathbb R$. We first prove the needed [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). Let $p$ be a real-valued [sublinear function](../../../../../sublinear-function.md) on $X$, meaning $p(a+b)\leq p(a)+p(b)$ and $p(ta)=tp(a)$ for $t\geq0$, and let $g$ be linear on a [vector subspace](../../../../../vector-subspace.md) $M$, with $g(m)\leq p(m)$. To extend across $v\notin M$, write

$$
\widetilde g(m+tv)=g(m)+tc.
$$

The necessary bounds on $c$ are

$$
L=\sup_{m\in M}\bigl[g(m)-p(m-v)\bigr]\leq c\leq\inf_{n\in M}\bigl[p(n+v)-g(n)\bigr]=U.
$$

They are compatible because

$$
g(m)+g(n)=g(m+n)\leq p(m+n)\leq p(m-v)+p(n+v).
$$

Taking one variable equal to zero also shows that $L,U$ are finite. Choose $c\in[L,U]$. The upper bound proves domination when $t>0$, after dividing $m+tv$ by $t$; the lower bound proves it when $t<0$, after dividing by $-t$. Thus $\widetilde g\leq p$ on $M+\mathbb Rv$. This is the [one-dimensional dominated extension of a real linear functional](../../../../../one-dimensional-dominated-extension-of-a-real-linear-functional.md).

Order all dominated extensions of $g$ by extension of their domains. A chain has an upper bound obtained by taking the union of the domains and [linear functionals](../../../../../linear-functional.md). [Zorn's lemma](../../../../../zorn-s-lemma.md) gives a maximal extension, and the one-dimensional construction shows that its domain must be all of $X$. We have therefore proved the real dominated-extension theorem. In particular, when $p$ is a [seminorm](../../../../../seminorm.md), domination at both $x$ and $-x$ gives **$|f(x)|\leq p(x)$**.

For $x_0\neq0$, choose a continuous [seminorm](../../../../../seminorm.md) $p$ with $p(x_0)>0$, and define $g(tx_0)=tp(x_0)$ on its one-dimensional span. Then $|g(tx_0)|\leq p(tx_0)$. Extend by the theorem just proved to $f$ with $|f(x)|\leq p(x)$. This bound makes $f$ continuous, and $f(x_0)=p(x_0)>0$. Applying this to the difference of two distinct points proves that **$X^*$ separates the points of $X$**, the [continuous-dual separation theorem for Hausdorff locally convex spaces](../../../../../continuous-dual-separation-theorem-for-hausdorff-locally-convex-spaces.md).

For separation from a [closed linear subspace](../../../../../closed-vector-subspace.md), choose a basic balanced neighborhood $V$ of zero such that $(x_0+V)\cap Y=\varnothing$. Write

$$
V=\{x:q(x)<1\},\qquad q(x)=\max_{1\leq i\leq m}\frac{p_i(x)}{\varepsilon_i}.
$$

Then $q(x_0-y)\geq1$ for every $y\in Y$. On $Y+\mathbb Rx_0$, define $g(y+tx_0)=t$, which is well-defined since $x_0\notin Y$. For $t\neq0$,

$$
q(y+tx_0)=|t|q(x_0+y/t)\geq|t|=|g(y+tx_0)|;
$$

for $t=0$ the inequality is immediate. The proved extension theorem gives a continuous $f$ dominated by $q$, with

$$
\boxed{f(x_0)=1,\qquad f|_Y=0.}
$$

This proves [separation of a point from a closed linear subspace](../../../../../separation-of-a-point-from-a-closed-linear-subspace.md) without using any unproved Hahn-Banach extension or separation result.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
