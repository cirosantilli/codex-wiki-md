<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

For finite-valued [discrete random variables](../../../../../random-variable-split.md), the [conditional entropy](../../../../../conditional-entropy.md) is

$$
H(X\mid Y)
=\sum_y\mathbb P(Y=y)H(X\mid Y=y)
=-\sum_{x,y}p(x,y)\log_2p(x\mid y).
$$

The [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md) in two orders gives

$$
H(X,Z\mid Y)
=H(X\mid Y)+H(Z\mid X,Y)
=H(Z\mid Y)+H(X\mid Y,Z).
$$

Therefore

$$
H(X\mid Y)
=H(X\mid Y,Z)+H(Z\mid Y)-H(Z\mid X,Y)
\leq H(X\mid Y,Z)+H(Z),
$$

using nonnegativity of conditional entropy and the fact that [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md). This proves the required inequality.

For [Fano's inequality](../../../../../fano-s-inequality.md), let $X$ take values in an alphabet of size $m$, let $\widehat X=g(Y)$ be any estimator, and put

$$
E=\boldsymbol1_{\{\widehat X\ne X\}},
\qquad p_e=\mathbb P(E=1).
$$

Because $E$ is determined by $(X,Y)$,

$$
H(X\mid Y)=H(E,X\mid Y)
=H(E\mid Y)+H(X\mid E,Y).
$$

Now $H(E\mid Y)\leq H(E)=h_2(p_e)$. If $E=0$, $X$ is determined by $Y$; if $E=1$, at most $m-1$ values remain possible. Hence

$$
H(X\mid E,Y)
\leq p_e\log_2(m-1).
$$

Combining the bounds yields

$$
\boxed{H(X\mid Y)
\leq h_2(p_e)+p_e\log_2(m-1)}.
$$

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
