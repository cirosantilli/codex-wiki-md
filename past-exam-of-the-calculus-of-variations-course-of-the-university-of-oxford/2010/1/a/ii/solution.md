<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [strong local minimizer of a variational integral](../../../../../strong-local-minimizer-of-a-variational-integral.md) is an admissible $\bar u$ for which some $\rho>0$ satisfies

$$
\boxed{I(v)\geq I(\bar u)\quad\text{for }v\in\mathcal A\text{ with }\|v-\bar u\|_\infty<\rho.}
$$

Only the function values must be close; admissible derivatives may be large. Every strong local minimizer is therefore also a [weak local minimizer of a variational integral](../../../../../weak-local-minimizer-of-a-variational-integral.md).

A [point of convexity](../../../../../point-of-convexity.md) of $g\in C^1(\mathbb R)$ is a point $v_0$ where its tangent line supports the entire graph from below:

$$
g(v)\geq g(v_0)+g'(v_0)(v-v_0)\quad\text{for every }v\in\mathbb R.
$$

The [Weierstrass necessary condition](../../../../../weierstrass-necessary-condition.md) says that, at almost every $x$, $\bar u'(x)$ is a [point of convexity](../../../../../point-of-convexity.md) of $v\mapsto f(x,\bar u(x),v)$. In terms of the [Weierstrass excess function](../../../../../weierstrass-excess-function.md),

$$
E(x,\bar u,\bar u',v)=f(x,\bar u,v)-f(x,\bar u,\bar u')-f_v(x,\bar u,\bar u')(v-\bar u')\geq0\quad(v\in\mathbb R).
$$

Now use the stated [derivative](../../../../../derivative.md) [coercivity](../../../../../coercive-function.md). If $\bar u$ were not a local minimizer in $L^1$, there would be $v_n\in\mathcal A$ with $\|v_n-\bar u\|_1\to0$ and $I(v_n)<I(\bar u)$. The energy bound gives

$$
c\int_a^b|v_n'|^{2010}\,dx\leq I(\bar u)+d(b-a).
$$

The common value $v_n(a)=\alpha$ controls their function norms as well, by $|v_n(x)|\leq|\alpha|+\int_a^b|v_n'|$. Thus $(v_n)$ is bounded in $W^{1,2010}(a,b)$. The one-dimensional compact [Sobolev embedding](../../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md) into $C([a,b])$ supplies a uniformly convergent subsequence. Its limit must be $\bar u$, since the same subsequence converges to $\bar u$ in $L^1$. Eventually $\|v_n-\bar u\|_\infty<\rho$, contradicting strong local minimality. Hence **$\bar u$ is also a local minimizer in $L^1$**. This is [coercivity transfers strong minimality to L1 minimality](../../../../../coercivity-transfers-strong-minimality-to-l1-minimality.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
