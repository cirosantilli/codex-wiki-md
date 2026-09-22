<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the physical diffusion and consumption constants $D,k>0$. Use the [travelling wave](../../../../../../travelling-wave.md) coordinate $z=x-vt$, with $v>0$. Then $\partial_t=-v\,d/dz$ and $\partial_x=d/dz$. The original PDF has the bacterial drift flux $\chi b c_x$: the TeX transcription's $\chi^b$ is erroneous. Substituting the [logarithmic chemotactic sensitivity](../../../../../../logarithmic-chemotactic-sensitivity.md) $\chi=\alpha/C$ gives

$$
\boxed{-vB'=DB''-\alpha\left(\frac{BC'}{C}\right)',\qquad
vC'=kB.}
$$

Primes here denote differentiation with respect to $z$. The second equation already shows that nutrient increases towards the front whenever the bacterial density is positive. For the positive band, $C>0$ at every finite $z$, so division by $C$ is legitimate, despite its zero limit far behind.

Integrating the first equation once gives

$$
DB'+vB-\alpha\frac{BC'}{C}=J,
$$

with constant $J$. For a localized band with no bacterial flux at infinity, $B$ and its flux terms vanish ahead, so $J=0$. Equivalently the laboratory flux $-DB'+\alpha BC'/C$ equals $vB$. The [Keller--Segel model](../../../../../../keller-segel-model.md) then has the useful first-order reduction

$$
\boxed{\frac{B'}B=\frac\alpha D\frac{C'}C-\frac vD,\qquad
C'=\frac kv B.}
$$

The far-field conditions choose this zero-flux integration constant; it should not be imposed for an arbitrary nonlocalized travelling solution. We solve its positive localized branch in the next part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
