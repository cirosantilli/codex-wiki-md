<h1 id="15g/solution">Solution</h1>

↑ **Parent:** [15G](../15g.md)

A [norm](../../../../../norm.md) $p$ is nonnegative with $p(x)=0$ exactly when $x=0$, satisfies $p(ax)=|a|p(x)$, and obeys $p(x+y)\leq p(x)+p(y)$. The [Euclidean norm](../../../../../euclidean-norm.md) has positivity and absolute homogeneity immediately. For the [triangle inequality](../../../../../triangle-inequality.md), positivity of $\|x-ty\|_2^2$ for all real $t$ gives the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) $|x\cdot y|\leq\|x\|_2\|y\|_2$ (with $y=0$ immediate). Hence

$$
\|x+y\|_2^2\leq\|x\|_2^2+2\|x\|_2\|y\|_2+\|y\|_2^2,
$$

which proves the [triangle inequality](../../../../../triangle-inequality.md) after taking square roots.

For the prescribed set, use the [Minkowski functional](../../../../../minkowski-functional.md)

$$
\boxed{p_U(x)=\inf\{t>0:x\in tU\}.}
$$

Since $U$ is open and contains zero, some [Euclidean ball](../../../../../euclidean-ball.md) of radius $r>0$ lies inside it. Since it is bounded, it lies inside a ball of radius $R$. These inclusions imply $\|x\|_2/R\leq p_U(x)\leq\|x\|_2/r$, so the functional is finite and positive for nonzero $x$; it is zero at zero. Symmetry gives $p_U(-x)=p_U(x)$, and substitution in the infimum gives $p_U(ax)=a p_U(x)$ for $a>0$, hence absolute homogeneity for all real scalars.

Convexity and $0\in U$ imply $sU\subseteq U$ for $0\leq s\leq1$. Consequently, for $a>p_U(x)$ and $b>p_U(y)$, one has $x/a,y/b\in U$. Convexity then gives

$$
\frac{x+y}{a+b}=\frac a{a+b}\frac xa+\frac b{a+b}\frac yb\in U,
$$

so $p_U(x+y)\leq a+b$. Letting $a\downarrow p_U(x)$ and $b\downarrow p_U(y)$ proves the [triangle inequality](../../../../../triangle-inequality.md).

Finally, if $p_U(x)<1$, there is a $t<1$ with $x\in tU\subseteq U$. Conversely, if $x\in U$ and $x\ne0$, openness permits $(1+\delta)x\in U$ for some $\delta>0$, so $p_U(x)\leq1/(1+\delta)<1$; zero is immediate. Thus **$\boxed{U=\{x:p_U(x)<1\}}$**, completing the [norm from a bounded symmetric convex neighbourhood](../../../../../norm-from-a-bounded-symmetric-convex-neighbourhood.md) construction.

## ↑ Ancestors (10)

1. [15G](../15g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
