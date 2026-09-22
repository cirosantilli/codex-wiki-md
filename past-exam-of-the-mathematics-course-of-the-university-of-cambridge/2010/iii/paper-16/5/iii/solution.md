<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the [affine scheme](../../../../../../affine-scheme.md) $X=\mathbb A^1_k$, its [function field](../../../../../../function-field-of-an-algebraic-variety.md) $K=k(t)$, and the [constant sheaf](../../../../../../constant-sheaf.md) $\mathcal K$ with value $K$. By Question 4(ii), $\mathcal K$ is a [flasque sheaf](../../../../../../flasque-sheaf.md). At the two distinct closed rational points $p_0=0$ and $p_1=1$, let $S_0,S_1$ be [skyscraper sheaves](../../../../../../skyscraper-sheaf.md) with value $K$: on an open subset $V$, $S_i(V)=K$ if $p_i\in V$ and is zero otherwise. Both are [flasque sheaves](../../../../../../flasque-sheaf.md).

There is a natural [morphism of sheaves](../../../../../../morphism-of-sheaves.md)

$$
\rho:\mathcal K\longrightarrow S_0\oplus S_1,
$$

which sends a constant rational function to the same element in every summand present on the open subset. At $p_i$, its [stalk](../../../../../../stalk-of-a-sheaf.md) map is the identity $K\to K$, and at any other point the target [stalk](../../../../../../stalk-of-a-sheaf.md) is zero. Thus $\rho$ is a surjection of [sheaves](../../../../../../sheaf-mathematics.md), although it is not surjective on [global sections](../../../../../../global-section.md). Put $\mathcal F=\ker\rho$.

This can even be an example of [sheaves](../../../../../../sheaf-mathematics.md) of $\mathcal O_X$-[modules](../../../../../../module-mathematics.md): let [regular functions](../../../../../../regular-function.md) act on each copy of $K$ by multiplication after embedding them in $K$. At the closed points this action is multiplication by a rational function, not evaluation at the point. With these actions, $\rho$ is $\mathcal O_X$-linear.

The exact sequence $0\to\mathcal F\to\mathcal K\to S_0\oplus S_1\to0$, together with [flasque](../../../../../../flasque-sheaf.md) acyclicity, gives

$$
0\longrightarrow H^0(X,\mathcal F)\longrightarrow K\xrightarrow{a\mapsto(a,a)}K^2\longrightarrow H^1(X,\mathcal F)\longrightarrow0.
$$

Hence $H^0(X,\mathcal F)=0$ and $H^1(X,\mathcal F)=K^2/\Delta K\simeq K\ne0$. In contrast, use the one-member [affine open cover](../../../../../../affine-open-cover.md) $\mathcal U=\{X\}$. Its alternating [Čech cochain complex](../../../../../../cech-cochain-complex.md) has no positive-degree terms, so $\check H^1(\mathcal U,\mathcal F)=0$. We have the explicit discrepancy

$$
\boxed{\check H^1(\{X\},\mathcal F)=0\ne H^1(X,\mathcal F)\simeq k(t).}
$$

The [sheaf](../../../../../../sheaf-mathematics.md) $\mathcal F$ is not a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md), as also follows from its nonzero higher [sheaf cohomology](../../../../../../sheaf-cohomology.md) on an [affine scheme](../../../../../../affine-scheme.md). Thus this example does not contradict the [acyclic cover theorem](../../../../../../leray-s-theorem.md) for [quasi-coherent sheaves](../../../../../../quasi-coherent-sheaf.md) on affine covers.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
