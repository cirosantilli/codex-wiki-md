<h1 id="31j/solution">Solution</h1>

↑ **Parent:** [31J](../31j.md)

For points $x_1,\ldots,x_n\in\mathcal X$, the restriction of $\mathcal H$ to those points is the set of binary vectors

$$
\mathcal H|_{x_{1:n}}
=\{(h(x_1),\ldots,h(x_n)):h\in\mathcal H\}.
$$

The [shattering coefficient](../../../../../shattering-coefficient.md) is

$$
\boxed{
s(\mathcal H,n)
=\sup_{x_1,\ldots,x_n\in\mathcal X}
|\mathcal H|_{x_{1:n}}|}.
$$

The [VC dimension](../../../../../vc-dimension.md) is

$$
\boxed{
\operatorname{VC}(\mathcal H)
=\sup\{n:s(\mathcal H,n)=2^n\}},
$$

with value infinity when arbitrarily large finite sets are shattered.

If $\mathcal H'\subseteq\mathcal H$, then for every choice of points,

$$
\mathcal H'|_{x_{1:n}}\subseteq\mathcal H|_{x_{1:n}}.
$$

Thus every set shattered by $\mathcal H'$ is also shattered by $\mathcal H$, and

$$
\operatorname{VC}(\mathcal H')\leq\operatorname{VC}(\mathcal H).
$$

Now put $d=\dim\mathcal F$ and suppose that $x_1,\ldots,x_n$ are shattered by

$$
\mathcal H
=\{\mathbf1_{\{u:f(u)\leq0\}}:f\in\mathcal F'\}.
$$

Consider the [linear map](../../../../../linear-map.md)

$$
T:\mathcal F\longrightarrow\mathbb R^n,
\qquad
Tf=(f(x_1),\ldots,f(x_n)).
$$

If $n>d$, the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) shows that $\operatorname{im}T$ is a proper subspace of $\mathbb R^n$. Choose a nonzero

$$
\alpha\in(\operatorname{im}T)^\perp
$$

and replace $\alpha$ by $-\alpha$ if necessary so that at least one coordinate is positive.

Ask for the labeling that assigns label zero when $\alpha_i>0$ and label one when $\alpha_i<0$; coordinates with $\alpha_i=0$ may be labeled arbitrarily. Shattering would supply $f\in\mathcal F'$ such that

$$
\alpha_i>0\Longrightarrow f(x_i)>0,
\qquad
\alpha_i<0\Longrightarrow f(x_i)\leq0.
$$

Every product $\alpha_i f(x_i)$ is then nonnegative, and at least one is strictly positive. Hence

$$
\alpha\cdot Tf>0,
$$

contradicting $\alpha\perp\operatorname{im}T$. Therefore $n\leq d$, proving

$$
\boxed{\operatorname{VC}(\mathcal H)\leq\dim\mathcal F}.
$$

This is the [VC dimension of a vector space](../../../../../vc-dimension-of-a-vector-space.md) argument.

Finally, a closed [Euclidean ball](../../../../../euclidean-ball.md) with center $c$ and radius $r$ is

$$
\{x:\lVert x-c\rVert_2^2\leq r^2\}
=\{x:f_{c,r}(x)\leq0\},
$$

where

$$
f_{c,r}(x)
=\lVert x\rVert_2^2-2c^Tx+\lVert c\rVert_2^2-r^2.
$$

Every such function lies in

$$
\mathcal F
=\operatorname{span}
\{\lVert x\rVert_2^2,x_1,\ldots,x_d,1\},
$$

whose dimension is at most $d+2$. Applying the result just proved gives the [VC dimension upper bound for Euclidean balls](../../../../../vc-dimension-upper-bound-for-euclidean-balls.md)

$$
\boxed{\operatorname{VC}(\mathcal H)\leq d+2}.
$$

## ↑ Ancestors (10)

1. [31J](../31j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
