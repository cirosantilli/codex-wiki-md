<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p_C(x)=\inf\{t>0:x\in tC\}$ be the [Minkowski functional](../../../../../../minkowski-functional.md) of $C$. Openness, convexity, and $0\in C$ make $p_C$ sublinear, with $p_C(x)<1$ for $x\in C$ and $p_C(x_0)\geq1$. Define a linear functional on $\mathbb Rx_0$ by $f(tx_0)=t p_C(x_0)$. The real [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) extends it to $X$ with $f\leq p_C$. Hence

$$
f(x)<1\leq f(x_0)
\qquad(x\in C).
$$

Apply this separation to the open ball of radius $\lVert x_0\rVert$ and rescale to obtain $f\in S_{X^*}$ with $f(x_0)=\lVert x_0\rVert$. For a closed subspace $Y$, apply it to

$$
C=Y+\{x:\lVert x\rVert<d(x_0,Y)\}.
$$

The separator must vanish on $Y$ because $C$ contains every translate along $Y$, and normalization gives

$$
Y\subseteq\ker f,
\qquad
f(x_0)=d(x_0,Y).
$$

Let $F\subseteq X^*$ be finite-dimensional and $\Phi\in B_{X^{**}}$. Consider

$$
S:X\to F^*,
\qquad
Sx(f)=f(x).
$$

If $\Phi|_F$ did not belong to $S((1+\varepsilon)B_X)$, finite-dimensional strict separation would produce some $f\in F$ with

$$
\Phi(f)>(1+\varepsilon)\sup_{x\in B_X}f(x)
=(1+\varepsilon)\lVert f\rVert,
$$

contradicting $\lVert\Phi\rVert\leq1$. Thus there is $x\in X$ with $\lVert x\rVert<1+\varepsilon$ and $f(x)=\Phi(f)$ for every $f\in F$.

Given a basic weak-star neighbourhood of $\Phi$ in $B_{X^{**}}$, apply this result to the finite-dimensional span of its defining functionals and then replace $x$ by $x/(1+\varepsilon)$. As $\varepsilon\downarrow0$, the resulting points of $J(B_X)$ enter that neighbourhood. Hence $J(B_X)$ is weak-star dense in $B_{X^{**}}$, proving [Goldstine theorem](../../../../../../goldstine-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
