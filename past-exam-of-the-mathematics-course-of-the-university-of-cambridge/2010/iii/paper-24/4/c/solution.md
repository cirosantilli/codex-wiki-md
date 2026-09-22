<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $L=\mathbb Q_p(\zeta_p)$, put $\pi=\zeta_p-1$. The [polynomial](../../../../../../polynomial-split.md)

$$
\Phi_p(1+T)=\frac{(1+T)^p-1}{T}
$$

is [Eisenstein](../../../../../../eisenstein-criterion.md) at $p$. It gives $[L:\mathbb Q_p]=e=p-1$, total ramification, and $v_L(\pi)=1$. Also $\mathcal O_L=\mathbb Z_p[\pi]$: in the power [basis](../../../../../../basis.md), terms $c_i\pi^i$ have [valuations](../../../../../../valuation.md) $(p-1)v_p(c_i)+i$ in different residue classes modulo $p-1$, so cannot cancel at the minimum. Integrality forces all $c_i$ integral.

Use part (b) with $\Phi_p(T)$ and differentiate the quotient at $\zeta_p$:

$$
\Phi'_p(\zeta_p)=\frac{p\zeta_p^{p-1}}{\zeta_p-1}.
$$

The [root of unity](../../../../../../root-of-unity.md) is a [unit](../../../../../../unit-in-a-ring.md), while $v_L(p)=p-1$ and $v_L(\pi)=1$. Hence the [cyclotomic local different exponent](../../../../../../cyclotomic-local-different-exponent.md) is

$$
\boxed{\delta(\mathbb Q_p(\zeta_p)/\mathbb Q_p)=p-2.}
$$

This includes $p=2$: that extension is trivial and the exponent is zero.

For $m=p^2-1$, construct an unramified quadratic extension $E/\mathbb Q_p$ by lifting an irreducible [quadratic polynomial](../../../../../../quadratic-polynomial.md) over $\mathbb F_p$. Its [residue field](../../../../../../residue-field.md) is $\mathbb F_{p^2}$. Each of its nonzero residue elements is a simple [polynomial root](../../../../../../root-of-a-polynomial.md) of $T^m-1$, so [Hensel's lemma](../../../../../../hensel-s-lemma.md) lifts all $m$ [polynomial roots](../../../../../../root-of-a-polynomial.md) into $E$. A primitive residue element lifts to a primitive mth [polynomial root](../../../../../../root-of-a-polynomial.md): its reduction already has order $m$, and its mth power is one.

Such a primitive [polynomial root](../../../../../../root-of-a-polynomial.md) cannot generate a proper subfield of $E$, since its residue has order $p^2-1>p-1$ and therefore generates the quadratic residue extension. Thus $\mathbb Q_p(\zeta_m)=E$ is unramified of degree two. Part (a) gives $\mathcal O_E=\mathbb Z_p[\zeta_m]$. The reduced [minimal polynomial of an algebraic element](../../../../../../minimal-polynomial-of-an-algebraic-element.md) has degree two and is separable, so its derivative at $\zeta_m$ is a [unit](../../../../../../unit-in-a-ring.md). Part (b) gives

$$
\boxed{\delta(\mathbb Q_p(\zeta_{p^2-1})/\mathbb Q_p)=0.}
$$

Both answers use normalized [discrete valuations](../../../../../../discrete-valuation.md) on the top [field](../../../../../../field.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
