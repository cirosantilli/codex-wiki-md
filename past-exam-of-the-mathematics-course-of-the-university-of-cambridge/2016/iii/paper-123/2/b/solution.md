<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $a=\sqrt[3]{3}$ and let $\zeta$ be a primitive cube root of unity. The [splitting field](../../../../../../splitting-field.md) is $L=\mathbb Q_3(a,\zeta)$. The [polynomial](../../../../../../polynomial-split.md) $X^3-3$ is an [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md), so $[\mathbb Q_3(a):\mathbb Q_3]=3$. Meanwhile $(1+2\zeta)^2=-3$ shows that $\mathbb Q_3(\zeta)$ is quadratic: $-3$ is not a square because its [valuation](../../../../../../valuation.md) is odd. A quadratic field cannot lie in the degree-three field. Consequently $[L:\mathbb Q_3]=6$, and the action on the three roots identifies its [Galois group](../../../../../../galois-group.md) with the [symmetric group](../../../../../../symmetric-group.md) $S_3$.

A useful [uniformizer](../../../../../../uniformizer.md) is

$$
\pi=\frac{\zeta-1}{a}.
$$

Since $(\zeta-1)^3=-3\zeta(\zeta-1)$, we obtain

$$
\pi^3=-\zeta(\zeta-1)=1+2\zeta,\qquad\pi^6=-3.
$$

Thus $\pi$ is a root of the [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) $X^6+3$. Its degree is six, so $L=\mathbb Q_3(\pi)$, the extension is totally ramified, and $\pi$ is a [uniformizer](../../../../../../uniformizer.md). With $v_L(\pi)=1$,

$$
v_L(3)=6,\qquad v_L(a)=2,\qquad v_L(\zeta-1)=3.
$$

This is the [Eisenstein sextic presentation of the splitting field of X3 minus 3 over Q3](../../../../../../eisenstein-sextic-presentation-of-the-splitting-field-of-x3-minus-3-over-q3.md).

Let $\tau(a)=\zeta a$, $\tau(\zeta)=\zeta$, and let $s(a)=a$, $s(\zeta)=\zeta^{-1}$. Then $\tau$ has order three, $s$ has order two, and $s\tau s=\tau^{-1}$. Their actions on the [uniformizer](../../../../../../uniformizer.md) are

$$
\tau(\pi)=\zeta^{-1}\pi,\qquad s(\pi)=-\zeta^{-1}\pi.
$$

The two nonidentity elements of $\langle\tau\rangle$ therefore satisfy

$$
v_L(\tau(\pi)-\pi)=v_L(\tau^2(\pi)-\pi)=1+v_L(\zeta-1)=4.
$$

Each transposition sends $\pi$ to $-\zeta^j\pi$ for some $j$, so its displacement has [valuation](../../../../../../valuation.md) one: $1+\zeta^j$ is a unit, reducing to $2$ modulo the [maximal ideal](../../../../../../maximal-ideal.md). The [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) now gives

$$
\boxed{G_{-1}=G_0=S_3,\qquad G_1=G_2=G_3=\langle\tau\rangle\cong C_3,\qquad G_i=1\ (i\geq4).}
$$

For real indices, this is $S_3$ on $[-1,0]$, $C_3$ on $(0,3]$, and $1$ for $t>3$. In particular the lower breaks are $0$ and $3$.

On $(0,3]$ the index $[G_0:G_t]$ is two; beyond three it is six. Thus the [Herbrand function](../../../../../../herbrand-function.md) is

$$
\varphi(t)=\begin{cases}t,&-1\leq t\leq0,\\t/2,&0\leq t\leq3,\\3/2+(t-3)/6,&t\geq3.\end{cases}
$$

The positive lower break $3$ becomes the upper break $3/2$. Therefore

$$
\boxed{G^u=\begin{cases}S_3,&-1\leq u\leq0,\\C_3,&0<u\leq3/2,\\1,&u>3/2.\end{cases}}
$$

The fractional upper break is allowed because the full extension is nonabelian. As a check, the [different exponent from ramification groups](../../../../../../different-exponent-from-ramification-groups.md) is $5+3\cdot2=11$. The derivative of the [minimal polynomial](../../../../../../minimal-polynomial.md) $X^6+3$ gives the same result: $v_L(6\pi^5)=6+5=11$. This is the $p=3$ case of [ramification groups of the splitting field of Xp minus p over the p-adic numbers](../../../../../../ramification-groups-of-the-splitting-field-of-xp-minus-p-over-the-p-adic-numbers.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
