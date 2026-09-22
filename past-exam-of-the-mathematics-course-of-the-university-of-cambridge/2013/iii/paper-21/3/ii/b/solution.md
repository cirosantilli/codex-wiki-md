<h1 id="3/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\alpha=\sqrt[3]{3}$ and $\zeta=\zeta_3$. The cubic is [Eisenstein](../../../../../../../eisenstein-criterion.md) and adjoining $\zeta$ adds at most a quadratic extension, so $[L:\mathbb Q_3]\leq6$. Set

$$
\pi=\frac{\zeta-1}{\alpha}.
$$

Using $\zeta^2+\zeta+1=0$ and $\alpha^3=3$, compute $\pi^3=1+2\zeta$ and $\pi^6=-3$. Thus $\pi$ satisfies the [Eisenstein polynomial](../../../../../../../eisenstein-polynomial.md) $X^6+3$. This proves $L=\mathbb Q_3(\pi)$, degree six, with $\pi$ a [uniformiser](../../../../../../../uniformizer.md) and the extension [totally ramified](../../../../../../../totally-ramified-extension.md). It is the splitting field of $X^3-3$, so its [Galois group](../../../../../../../galois-group.md) is $S_3$. This is the [Eisenstein sextic presentation of the splitting field of X3 minus 3 over Q3](../../../../../../../eisenstein-sextic-presentation-of-the-splitting-field-of-x3-minus-3-over-q3.md).

The six automorphisms have $\sigma(\alpha)=\zeta^a\alpha$, $a\in\{0,1,2\}$, and $\sigma(\zeta)=\zeta^b$, $b\in\{1,2\}$. Since $v_L(3)=6$, we have $v_L(\alpha)=2$ and $v_L(\zeta-1)=3$.

If $b=1$ and $a\ne0$, then $\sigma(\pi)=\zeta^{-a}\pi$, whence $v_L(\sigma(\pi)-\pi)=1+3=4$. These are the two nonidentity elements of the cyclic subgroup $C_3$.

If $b=2$, use $\zeta^2-1=(\zeta-1)(\zeta+1)=-(\zeta-1)\zeta^2$. Then $\sigma(\pi)=-\zeta^{2-a}\pi$. The coefficient $-\zeta^{2-a}-1$ reduces to $-2\ne0$ in the [residue field](../../../../../../../residue-field.md) $\mathbb F_3$, so the difference has [valuation](../../../../../../../valuation.md) one. These three automorphisms are the transpositions.

The [uniformizer criterion for lower ramification groups](../../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) consequently gives

$$
\boxed{G_{-1}=G_0=S_3,\qquad G_1=G_2=G_3=C_3,\qquad G_i=\{1\}\ (i\geq4).}
$$

As a consistency check, the [different exponent](../../../../../../../different-exponent.md) is $(6-1)+3(3-1)=11$. The derivative of the monogenic [Eisenstein polynomial](../../../../../../../eisenstein-polynomial.md) gives the same value, $v_L(6\pi^5)=6+5=11$. In particular, stopping the wild filtration at $G_1$ would give the wrong different.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 21](../../../../paper-21-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
