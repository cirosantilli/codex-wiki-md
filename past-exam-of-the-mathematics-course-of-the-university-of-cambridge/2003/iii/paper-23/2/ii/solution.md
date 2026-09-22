<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [local field](../../../../../../local-field.md) $F$ containing the Nth [roots of unity](../../../../../../root-of-unity.md), fix the [Local Artin map](../../../../../../local-artin-map.md) with arithmetic [Frobenius](../../../../../../frobenius-automorphism.md) convention. The [Hilbert norm residue symbol](../../../../../../hilbert-norm-residue-symbol.md) can be defined by

$$
(a,b)_{F,N}=\frac{\operatorname{rec}_F(b)(a^{1/N})}{a^{1/N}}\in\mu_N.
$$

It is independent of the chosen root, continuous and bimultiplicative, factors through $F^\times/(F^\times)^N$ in each variable, and gives a nondegenerate pairing on that finite [group](../../../../../../group-split.md). It satisfies $(a,b)_{F,N}=(b,a)_{F,N}^{-1}$ and $(a,1-a)_{F,N}=1$ for $a\ne1$. Its [norm](../../../../../../norm.md) interpretation is

$$
(a,b)_{F,N}=1\iff b\in N_{F(a^{1/N})/F}F(a^{1/N})^\times.
$$

For $N=2$ the [quadratic Hilbert symbol](../../../../../../quadratic-hilbert-symbol.md) is symmetric and sign-valued. It is also characterized by the existence of a nonzero solution of $z^2=ax^2+by^2$. Moreover $(a,-a)_F=1$, and therefore $(a,a)_F=(a,-1)_F$. We now compute both the [square-class groups](../../../../../../square-class-group-of-a-field.md) and the pairing explicitly.

For odd $p$, write $a=p^\alpha u$ with $u\in\mathbb Z_p^\times$. An element is a square exactly when $\alpha$ is even and the residue of $u$ is a square in $\mathbb F_p^\times$. Necessity follows by reduction; sufficiency follows from the simple-root form of [Hensel lemma](../../../../../../hensel-s-lemma.md) applied to $X^2-u$, since $2x$ is then a unit. If $\eta$ is any unit with nonsquare residue, this gives

$$
\boxed{\mathbb Q_p^\times/(\mathbb Q_p^\times)^2\cong C_2\times C_2,\qquad\text{representatives }1,\eta,p,\eta p\quad(p\text{ odd}).}
$$

The nonsquare unit defines an [unramified](../../../../../../unramified-extension.md) quadratic extension. Its [field norms](../../../../../../field-norm.md) include every unit and have even [valuation](../../../../../../valuation.md), as follows from the local norm calculation below. Thus $(\eta,u)_p=1$ for every unit, but $(\eta,p)_p=-1$. Finally $(p,p)_p=(p,-1)_p=(-1/p)$, by symmetry and the preceding unit calculation. Bimultiplicativity now proves [explicit quadratic Hilbert symbols over the p-adic numbers](../../../../../../explicit-quadratic-hilbert-symbols-over-the-p-adic-numbers.md):

$$
\boxed{(p^\alpha u,p^\beta v)_p=(-1)^{\alpha\beta(p-1)/2}\left(\frac up\right)^\beta\left(\frac vp\right)^\alpha\quad(p\text{ odd}).}
$$

Here the factors are [Legendre symbols](../../../../../../legendre-symbol.md) of the nonzero residues. The formula works for arbitrary integer [valuations](../../../../../../valuation.md) $\alpha,\beta$, since only their parity matters.

At $p=2$, the square of every odd integer is one modulo eight. Conversely, for an odd $u\equiv1\pmod8$, apply the [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) to $X^2-u$ at $1$: the error has [valuation](../../../../../../valuation.md) at least three, while the [derivative](../../../../../../derivative.md) has [valuation](../../../../../../valuation.md) one. Thus the [unit square classes of the p-adic integers](../../../../../../unit-square-classes-of-the-p-adic-integers.md) are precisely their four residues modulo eight. Combining this with parity of the [valuation](../../../../../../valuation.md) gives

$$
\boxed{\mathbb Q_2^\times/(\mathbb Q_2^\times)^2\cong C_2^3,\qquad\text{basis }[-1],[2],[5],\quad\text{representatives }\pm1,\pm2,\pm5,\pm10.}
$$

For an odd unit put

$$
\epsilon(u)=\frac{u-1}{2}\pmod2,\qquad\omega(u)=\frac{u^2-1}{8}\pmod2.
$$

Inspection of the residues $1,3,5,7$ gives $[u]=[-1]^{\epsilon(u)}[5]^{\omega(u)}$. It remains to compute six basis pairings. Explicit [field norms](../../../../../../field-norm.md) give

$$
(-1,2)_2=(-1,5)_2=(2,2)_2=(5,5)_2=1:
$$

indeed $2=1^2+1^2$, $5=1^2+2^2$, $2=2^2-2\cdot1^2$, and $5=5^2-5\cdot2^2$.

In contrast $(-1,-1)_2=-1$. To justify the obstruction even for rational 2-adic coordinates, write $x=2^t x_0$, $y=2^t y_0$ with $x_0,y_0$ integral and at least one odd. Then $v_2(x_0^2+y_0^2)$ is zero if exactly one is odd, and one if both are odd. A sum of squares equal to the unit $-1$ consequently forces $t=0$ and exactly one coordinate odd. Its residue modulo four would then be one, whereas $-1$ is three.

Similarly $(2,5)_2=-1$. If $x^2-2y^2$ is a unit, the [valuations](../../../../../../valuation.md) of the two terms have opposite parity, so cannot cancel. It follows that $x$ is an odd integral element and $y$ is integral. Modulo eight its [norm](../../../../../../norm.md) is then $1$ or $7$, never $5$. These signs, symmetry, and bimultiplicativity give

$$
\boxed{(2^\alpha u,2^\beta v)_2=(-1)^{\epsilon(u)\epsilon(v)+\alpha\omega(v)+\beta\omega(u)}.}
$$

The two boxed formulas determine the [quadratic Hilbert symbol](../../../../../../quadratic-hilbert-symbol.md) on all nonzero elements, including every rational prime $p$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
