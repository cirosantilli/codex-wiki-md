<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

Choose a positive common denominator $d$ so that $x=a/d$ and $y=b/d$ with nonzero [integers](../../../../../integer.md) $a,b$. Put $h=\gcd(a,b)>0$. Every element of the generated [subgroup](../../../../../subgroup.md) has the form $(ma+nb)/d$, so it lies in $(h/d)\mathbb Z$. Conversely, [Bezout identity](../../../../../bezout-identity.md) gives [integers](../../../../../integer.md) $u,v$ with $ua+vb=h$, so $h/d$ belongs to the generated [subgroup](../../../../../subgroup.md). Consequently

$$
\boxed{N=(h/d)\mathbb Z\cong\mathbb Z,\qquad k\longmapsto kh/d.}
$$

This map is a bijective additive [group homomorphism](../../../../../group-homomorphism.md). It is the two-generator instance of a [finitely generated subgroup of the rational additive group](../../../../../finitely-generated-subgroup-of-the-rational-additive-group.md) being an [infinite cyclic group](../../../../../infinite-cyclic-group.md).

For the real example, take $x=1$ and $y=\sqrt2$. The [group homomorphism](../../../../../group-homomorphism.md) $(m,n)\mapsto m+n\sqrt2$ from $\mathbb Z^2$ onto the generated [subgroup](../../../../../subgroup.md) is injective because $\sqrt2$ is an [irrational number](../../../../../irrational-number.md). Thus this [subgroup](../../../../../subgroup.md) is isomorphic to $\mathbb Z^2$. More directly, if a single real number $t$ generated it, then $1=at$ and $\sqrt2=bt$ for [integers](../../../../../integer.md) $a\ne0,b$, giving $\sqrt2=b/a$, a contradiction. **The choice $1,\sqrt2$ generates a noncyclic additive [subgroup](../../../../../subgroup.md).**

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
