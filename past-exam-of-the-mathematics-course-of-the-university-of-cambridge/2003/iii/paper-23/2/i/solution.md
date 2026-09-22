<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\mathcal O$ for the [valuation ring](../../../../../../valuation-ring.md) of $K$, $\pi$ for a [uniformizer](../../../../../../uniformizer.md), $v(\pi)=1$, and $k=\mathbb F_q$ for the [residue field](../../../../../../residue-field.md). A useful [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) is the following: if $f\in\mathcal O[X]$ and $a_0\in\mathcal O$ satisfy

$$
v(f(a_0))>2v(f'(a_0)),
$$

then there is a root $a\in\mathcal O$ with $v(a-a_0)>v(f'(a_0))$, unique among roots in that ball. If $f(a_0)\ne0$, its distance satisfies $v(a-a_0)=v(f(a_0))-v(f'(a_0))$.

Here is a proof by successive correction. Put $s=v(f'(a_0))$, $d_j=v(f(a_j))$, and

$$
a_{j+1}=a_j-\frac{f(a_j)}{f'(a_j)}.
$$

Stop if a root has already been reached. Otherwise the correction has [valuation](../../../../../../valuation.md) $d_j-s>s$. Integral Taylor expansions show that $v(f'(a_{j+1}))=s$ and

$$
d_{j+1}\ge2(d_j-s),\qquad d_{j+1}-2s\ge2(d_j-2s).
$$

Thus $d_j-2s$ grows at least geometrically, the corrections tend to zero, and [completeness](../../../../../../completeness.md) gives a limit $a$ with $f(a)=0$. The first correction has strictly smaller [valuation](../../../../../../valuation.md) than every later nonzero correction, proving the asserted distance. If $x,y$ are in the ball $v(x-a_0),v(y-a_0)>s$, then

$$
f(x)-f(y)=(x-y)\bigl(f'(a_0)+c\bigr),\qquad v(c)>s.
$$

The second factor cannot vanish. Two roots in the ball must therefore coincide. This proves [Hensel lemma](../../../../../../hensel-s-lemma.md); in particular a simple root modulo $\pi$ has a unique lift with that residue.

We use this to establish [existence and uniqueness of unramified local extensions](../../../../../../existence-and-uniqueness-of-unramified-local-extensions.md). For each integer $d\ge1$, choose a monic [irreducible polynomial](../../../../../../irreducible-polynomial.md) $\bar f\in k[X]$ of degree $d$ and lift it to a monic $f\in\mathcal O[X]$. Reduction and [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) show that $f$ remains irreducible over $K$. Let

$$
A=\mathcal O[X]/(f),\qquad L=K[X]/(f).
$$

The [ring](../../../../../../ring.md) $A$ is finite free and complete over $\mathcal O$, and $A/\pi A\cong\mathbb F_{q^d}$. An element outside $\pi A$ is invertible: lift an inverse from the [residue field](../../../../../../residue-field.md) and invert the remaining $1+\pi z$ by a convergent geometric series. Every nonzero element of $A$ is $\pi^t$ times such a unit, since $\bigcap_t\pi^t A=0$ in a finite free [module](../../../../../../module-mathematics.md). Thus $A$ is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md), its fraction field is $L$, and

$$
[L:K]=d=[k_L:k],\qquad e(L/K)=1.
$$

This constructs an [unramified extension](../../../../../../unramified-extension.md) of each degree.

Conversely, let $M/K$ be an [unramified extension](../../../../../../unramified-extension.md) of degree $d$. Its [residue field](../../../../../../residue-field.md) is the unique degree-$d$ [finite field extension](../../../../../../finite-field-extension.md) $\mathbb F_{q^d}/\mathbb F_q$. Choose a residue root of $\bar f$ in it. The root is simple, so [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts it to a root of $f$ in $M$. This embeds $L$ into $M$, and equality of degrees makes it an isomorphism. All $d$ residue conjugates lift in $L$ itself; hence $L/K$ is [Galois](../../../../../../finite-galois-extension.md), and reduction identifies its [Galois group](../../../../../../galois-group.md) with the cyclic [Galois group](../../../../../../galois-group.md) of the [residue field](../../../../../../residue-field.md) extension. Its distinguished [Frobenius automorphism](../../../../../../frobenius-automorphism.md) reduces to $x\mapsto x^q$.

**There is exactly one unramified extension $K_d$ of each degree inside a fixed algebraic closure**, and

$$
\boxed{\operatorname{Gal}(K_d/K)\cong C_d,\qquad K_d=K(\mu_{q^d-1}),\qquad K_a\subseteq K_b\iff a\mid b.}
$$

For the middle equality, every nonzero element of $\mathbb F_{q^d}$ lifts uniquely to a $(q^d-1)$st [root of unity](../../../../../../root-of-unity.md), because that exponent is prime to $p$. A primitive such residue generates the [finite field extension](../../../../../../finite-field-extension.md), so its lift generates $K_d$. Taking the union gives the [maximal unramified extension](../../../../../../maximal-unramified-extension.md), with [Galois group](../../../../../../galois-group.md) $\widehat{\mathbb Z}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
