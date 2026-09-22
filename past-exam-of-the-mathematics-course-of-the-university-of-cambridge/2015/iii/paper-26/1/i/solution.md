<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**A strong lifting lemma.** Let $R$ be a complete [discrete valuation ring](../../../../../../discrete-valuation-ring.md), with fraction field $F$ and normalized [discrete valuation](../../../../../../discrete-valuation.md) $v$. A useful [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) says that for $f\in R[T]$ and $a\in R$ satisfying

$$
v(f(a))>2v(f'(a)),
$$

there is a root $b\in R$ with

$$
\boxed{v(b-a)=v(f(a))-v(f'(a)).}
$$

If $f(a)=0$, take $b=a$. Otherwise the hypothesis ensures that $f'(a)\ne0$. The root is unique among $b$ satisfying $v(b-a)>v(f'(a))$. In particular, a simple root of the reduction of $f$ lifts uniquely with its specified residue.

Here is a proof by [Newton iteration over a valued field](../../../../../../newton-iteration-over-a-valued-field.md). Put $a_0=a$ and

$$
a_{j+1}=a_j-\frac{f(a_j)}{f'(a_j)}.
$$

Write $A_j=v(f(a_j))$ and $B=v(f'(a_0))$. Taylor expansion over $R$ shows, inductively, that the increment has [valuation](../../../../../../valuation.md) $A_j-B>B$, that $v(f'(a_{j+1}))=B$, and that

$$
A_{j+1}\geq2A_j-2B,\qquad A_j-2B\geq2^j(A_0-2B).
$$

Indeed, the constant and linear terms of $f(a_{j+1})$ cancel, leaving terms of [valuation](../../../../../../valuation.md) at least twice that of the increment. The change in $f'$ has [valuation](../../../../../../valuation.md) greater than $B$, so its [valuation](../../../../../../valuation.md) stays $B$. Thus all iterates lie in $R$ and form a Cauchy sequence. Completeness and continuity give a root $b$. The later increments have strictly larger [valuations](../../../../../../valuation.md) than the first, proving the displayed distance formula. For uniqueness, if $b,c$ are in the stated ball, Taylor expansion factors

$$
f(b)-f(c)=(b-c)\bigl(f'(a)+\eta\bigr),\qquad v(\eta)>B.
$$

The second factor is nonzero, so two roots must coincide. This proves [Hensel's lemma](../../../../../../hensel-s-lemma.md) in the form needed here.

**Odd [residue characteristic](../../../../../../residue-characteristic.md).** For odd $p$, a [p-adic unit](../../../../../../p-adic-unit.md) $u$ is a square exactly when its reduction is a square in $\mathbb F_p^\times$. Necessity follows by reduction. For sufficiency, a nonzero residue root of $T^2-u$ has derivative $2T$ invertible modulo $p$, so the [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts it. The [multiplicative group of a finite field is cyclic](../../../../../../multiplicative-group-of-a-finite-field-is-cyclic.md), and its subgroup of squares has index two. Therefore

$$
\boxed{\mathbb Z_p^\times/(\mathbb Z_p^\times)^2\cong C_2
\quad(p\text{ odd}).}
$$

Representatives are $1$ and any unit whose reduction is a quadratic nonresidue.

**[Residue characteristic](../../../../../../residue-characteristic.md) two.** An odd integer has square congruent to one modulo eight, so a square [2-adic unit](../../../../../../2-adic-unit.md) must lie in $1+8\mathbb Z_2$. Conversely, if $u\equiv1\pmod8$, take $f(T)=T^2-u$ and $a=1$. Then $v_2(f(1))\geq3>2v_2(f'(1))=2$, and the [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) produces a square root. Hence

$$
(\mathbb Z_2^\times)^2=1+8\mathbb Z_2,\qquad
\boxed{\mathbb Z_2^\times/(\mathbb Z_2^\times)^2
\cong(\mathbb Z/8\mathbb Z)^\times\cong C_2\times C_2.}
$$

The four [unit square classes of the p-adic integers](../../../../../../unit-square-classes-of-the-p-adic-integers.md) have representatives $1,3,5,7$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
