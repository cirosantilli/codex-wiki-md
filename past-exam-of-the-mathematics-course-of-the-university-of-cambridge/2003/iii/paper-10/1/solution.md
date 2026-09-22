<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Here “subspace” is understood to mean a closed [closed linear subspace](../../../../../closed-vector-subspace.md). Closedness matters: the [finitely supported sequences](../../../../../finitely-supported-sequence.md) $c_{00}$ are an infinite-dimensional algebraic subspace of $\ell^p$, but contain no infinite-dimensional complete subspace. Indeed, any such subspace would be the countable union of its intersections with the finite-dimensional coordinate spaces, contrary to the [Baire category theorem](../../../../../baire-category-theorem.md). We prove the assertion with the intended closedness convention, for $1\le p<\infty$.

Write $E=\ell^p$, the [l-p sequence space](../../../../../l-p-sequence-space.md). Choose positive numbers $\delta_n$ with $\sum_n2\delta_n<1$. Starting with $m_0=0$, choose $x_n\in X$ with $\|x_n\|_p=1$ and its first $m_{n-1}$ coordinates zero. This is possible because the kernel of finitely many coordinate [linear functionals](../../../../../linear-functional.md) on an infinite-dimensional [vector space](../../../../../vector-space-split.md) is still infinite-dimensional. Choose $m_n>m_{n-1}$ so that the part of $x_n$ after coordinate $m_n$ has norm below $\delta_n$. Let $v_n$ be its restriction to $I_n=(m_{n-1},m_n]$, and put $u_n=v_n/\|v_n\|_p$. The [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|x_n-u_n\|_p\le\|x_n-v_n\|_p+|1-\|v_n\|_p|<2\delta_n.
$$

The vectors $u_n$ form a normalized [block basic sequence](../../../../../block-basic-sequence.md). Their supports are disjoint, so

$$
\left\|\sum_n a_nu_n\right\|_p^p=\sum_n|a_n|^p.
$$

Consequently $U=\overline{\operatorname{span}}\{u_n\}$ is isometric to the [l-p sequence space](../../../../../l-p-sequence-space.md).

For each block choose a norm-one [linear functional](../../../../../linear-functional.md) $\phi_n$ supported on $I_n$ with $\phi_n(u_n)=1$. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) supplies such a functional, including when $p=1$. Define

$$
Qz=\sum_n\phi_n(z)u_n.
$$

The series converges in the [l-p sequence space](../../../../../l-p-sequence-space.md), since

$$
\|Qz\|_p^p=\sum_n|\phi_n(z)|^p\le\sum_n\|z|_{I_n}\|_p^p\le\|z\|_p^p.
$$

Also $Qu_n=u_n$, so $Q$ is a bounded projection onto $U$. Now define the [bounded linear operator](../../../../../continuous-linear-operator.md)

$$
A=I+\sum_n\phi_n(\cdot)(x_n-u_n).
$$

This series converges in [operator norm](../../../../../operator-norm.md) and $\|A-I\|\le\sum_n2\delta_n<1$. The [Neumann series](../../../../../neumann-series.md) therefore makes $A$ invertible. Disjoint support gives $Au_n=x_n$. Thus $Y=AU=\overline{\operatorname{span}}\{x_n\}$ lies in the closed subspace $X$, is isomorphic to the [l-p sequence space](../../../../../l-p-sequence-space.md), and is the range of the bounded projection $AQA^{-1}$ on the whole space $E$. This proves **the required copy of $\ell^p$ is complemented in the ambient $\ell^p$**, not just in $X$.

Now let $Z$ be an infinite-dimensional [complemented subspace](../../../../../complemented-subspace.md) of $E$. The construction supplies $Y\subset Z$ with $Y\cong E$ and a bounded projection $R:E\to Y$. Its restriction to $Z$ gives the topological [direct sum](../../../../../direct-sum.md)

$$
Z=Y\oplus W,\qquad W=Z\cap\ker R.
$$

If $P:E\to Z$ is a bounded projection, then $(I-R)P$ is a bounded projection onto $W$: its range lies in $W$, and it fixes every element of $W$. Hence $W$ is a [complemented subspace](../../../../../complemented-subspace.md) of $E$, so $E\cong W\oplus V$ for some closed $V$.

We give the absorption argument in the [Pełczyński decomposition method](../../../../../pelczynski-decomposition-method.md) explicitly. Reindexing coordinates by a bijection between $\mathbb N^2$ and $\mathbb N$ yields $E\cong(\bigoplus_{n\ge1}E)_p$. Applying the fixed [Banach space isomorphism](../../../../../banach-space-isomorphism.md) $E\cong W\oplus V$ in every coordinate gives

$$
E\oplus W
\cong\left(\bigoplus_{n\ge1}(W\oplus V)\right)_p\oplus W
\cong\left(\bigoplus_{n\ge1}W\right)_p\oplus\left(\bigoplus_{n\ge1}V\right)_p\oplus W
\cong E.
$$

The extra $W$ is absorbed by shifting the countably many $W$ summands. The maps are bounded with bounded inverses because the same two-space decomposition is used uniformly in each summand; we may equip each finite [direct sum](../../../../../direct-sum.md) with its equivalent $p$-sum norm. Since $Z\cong E\oplus W$, **$Z\cong\ell^p$**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
