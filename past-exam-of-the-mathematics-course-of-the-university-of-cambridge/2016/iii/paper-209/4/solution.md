<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $m=\mathbb E\|X_1\|_2$ and $q=\sqrt n\,K\geq2$. The [Lipschitz continuity](../../../../../lipschitz-continuity.md) of cosine and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) imply

$$
|S_n(u)-S_n(v)|\leq L_n\|u-v\|_2,\qquad
L_n=\sum_{k=1}^n\|X_k\|_2+nm,\qquad \mathbb E L_n=2nm.
$$

The centered expectation term contributes $nm$; omitting it would leave the [Lipschitz bound](../../../../../lipschitz-bound.md) incomplete. In particular $S_n$ has continuous sample paths on the compact cube, so its maximum exists and is measurable.

Put

$$
a=\frac{R^2-64d}{64(d+1)}>0,\qquad
\eta=\frac{1}{\sqrt n\,q^a}.
$$

Choose a Cartesian [finite net](../../../../../finite-net.md) $G\subset[-K,K]^d$ whose coordinate spacings are at most $\eta$, including the endpoints. Every point of the cube is within [Euclidean norm](../../../../../euclidean-norm.md) distance $\sqrt d\,\eta$ of $G$, and

$$
|G|\leq(2K/\eta+2)^d\leq4^d q^{d(1+a)}.
$$

On the event $L_n\leq nq^a$, replacing any $u$ by a nearby grid point changes $S_n$ by at most $\sqrt{dn}$. Since $R>8\sqrt d$ and $\log(nK^2)\geq\log4$, this is less than $\frac R4\sqrt{n\log(nK^2)}$. Therefore

$$
\left\{\max_u|S_n(u)|\geq\frac R2\sqrt{n\log(nK^2)}\right\}
\subseteq\{L_n>nq^a\}\cup
\bigcup_{v\in G}\left\{|S_n(v)|\geq\frac R4\sqrt{n\log(nK^2)}\right\}.
$$

The [Markov inequality](../../../../../markov-inequality.md) bounds the first event by $2m q^{-a}$. At a fixed $v$, the summands are centered, [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md), and have absolute value at most $2$. The supplied [Hoeffding inequality](../../../../../hoeffding-inequality.md), with $M=2$, bounds each grid event by

$$
2\exp\left(-\frac{R^2\log(nK^2)}{128}\right)=2q^{-R^2/64}.
$$

A [union bound](../../../../../boole-s-inequality.md) now gives

$$
\mathbb P\left(\max_u|S_n(u)|\geq\frac R2\sqrt{n\log(nK^2)}\right)
\leq2m q^{-a}+2\cdot4^d q^{d(1+a)-R^2/64}.
$$

The choice of $a$ balances the cost of a large random [Lipschitz constant](../../../../../lipschitz-constant.md) against the [covering number](../../../../../metric-covering-number.md) of the cube: $d(1+a)-R^2/64=-a$. Consequently **$C=2m+2\cdot4^d$ works**, with

$$
\boxed{\mathbb P\left(\max_{u\in[-K,K]^d}|S_n(u)|\geq\frac R2\sqrt{n\log(nK^2)}\right)
\leq(2m+2\cdot4^d)(\sqrt n\,K)^{(64d-R^2)/(64d+64)}.}
$$

This uses only the first moment $m$ and has a constant independent of $n,K,R$. The [finite net](../../../../../finite-net.md) is deterministic even though the [Lipschitz constant](../../../../../lipschitz-constant.md) is random.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 209](../../paper-209-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
