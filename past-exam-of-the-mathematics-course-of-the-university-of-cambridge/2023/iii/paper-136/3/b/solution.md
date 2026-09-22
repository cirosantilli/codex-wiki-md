<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\alpha$ be a root of

$$
f(X)=X^3+3X+3.
$$

The polynomial is Eisenstein at $3$, so $E=\mathbb Q_3(\alpha)$ is totally ramified of degree three and $\mathcal O_E=\mathbb Z_3[\alpha]$. Its discriminant is

$$
\Delta=-4\cdot3^3-27\cdot3^2=-351=-3^3\cdot13.
$$

Its odd valuation makes $\Delta$ nonsquare in $\mathbb Q_3$, so the [Galois group of an irreducible cubic](../../../../../../galois-group-of-an-irreducible-cubic.md) shows that the splitting field $L$ has Galois group $S_3$. The quadratic extension obtained by adjoining $\sqrt\Delta$ is ramified, so $L/\mathbb Q_3$ is totally ramified. Therefore

$$
G_{-1}=G_0=S_3,
\qquad
G_1=A_3,
$$

because the [wild inertia group](../../../../../../wild-inertia-group.md) is the unique Sylow $3$-subgroup of $S_3$.

It remains to find the wild break. Since

$$
f'(\alpha)=3(\alpha^2+1)
$$

and $\alpha^2+1$ is a unit, the [different ideal](../../../../../../different-ideal.md) of $E/\mathbb Q_3$ has exponent $v_E(f'(\alpha))=3$. The extension $L/E$ is a tamely ramified quadratic extension and has different exponent one. The [different in a tower](../../../../../../different-in-a-tower.md) therefore gives different exponent

$$
d(L/\mathbb Q_3)=1+2\cdot3=7.
$$

On the other hand, the [different exponent from ramification groups](../../../../../../different-exponent-from-ramification-groups.md) is

$$
7=\sum_{i\geq0}(|G_i|-1)
=5+2b,
$$

where $b$ is the last index for which $G_b=A_3$. Thus $b=1$, and

$$
\boxed{G_{-1}=G_0=S_3,\qquad G_1=A_3,\qquad G_i=1\quad(i\geq2).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
