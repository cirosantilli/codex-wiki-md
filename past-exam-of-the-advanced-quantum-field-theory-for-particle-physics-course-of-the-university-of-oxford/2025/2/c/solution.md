<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The middle panel in part [a](../a.md) has an internal [photon](../../../../photon.md) of [momentum](../../../../momentum-split.md) $k$ joining two points on a [fermion](../../../../fermion.md) line; the internal [fermion](../../../../fermion.md) has [momentum](../../../../momentum-split.md) $p-k$. It is a [one-particle-irreducible Feynman diagram](../../../../one-particle-irreducible-feynman-diagram.md) with no [closed fermion loop sign](../../../../closed-fermion-loop-sign.md). In [Feynman gauge](../../../../feynman-gauge.md),

$$
-i\Sigma(p)=\int_k(-ie\gamma^\alpha)
\frac{i(\not p-\not k+m)}{(p-k)^2-m^2+i0}
(-ie\gamma^\beta)\frac{-ig_{\alpha\beta}}{k^2+i0},
$$

or

$$
\boxed{\Sigma(p)=-ie^2\int_k
\frac{(2-d)(\not p-\not k)+dm}{[k^2+i0][(p-k)^2-m^2+i0]}.}
$$

The decomposition in the source gives $\operatorname{tr}(\not p\Sigma)=4p^2S(p^2)$. In particular,

$$
S(p^2)=-\frac{ie^2(d-2)}{p^2}\int_k
\frac{p\cdot k-p^2}{[k^2+i0][(p-k)^2-m^2+i0]}.
$$

For a direct [ultraviolet divergence](../../../../ultraviolet-divergence.md) extraction, use a [Feynman parameter](../../../../feynman-parameter.md) $x$ multiplying the massive denominator, shift $r=k-xp$, and define $\Delta=xm^2-x(1-x)p^2$. Then $\not p-\not k=(1-x)\not p-\not r$ and

$$
\int_0^1dx\int_r\frac1{(r^2-\Delta+i0)^2}
\bigg|_{\rm UV}=\frac{i}{16\pi^2\epsilon}\int_0^1dx.
$$

Odd $r$ terms integrate to zero. Taking the [trace](../../../../matrix-trace.md) explicitly supplies the weight $(2-d)(1-x)$, whose integral tends to $-1$. Hence

$$
\operatorname{tr}(\not p\Sigma)\big|_{\rm UV}
=-\frac{4e^2p^2}{16\pi^2\epsilon},\qquad
\boxed{S(p^2)\big|_{\rm UV}=-\frac{e^2}{16\pi^2\epsilon}.}
$$

As a check on the same [fermion self-energy](../../../../fermion-self-energy.md) calculation,

$$
\Sigma(p)\big|_{\rm UV}=\frac{e^2}{16\pi^2\epsilon}(-\not p+4m).
$$

This is the [ultraviolet pole of QED fermion self-energy](../../../../ultraviolet-pole-of-qed-fermion-self-energy.md). It is safe to extract it at generic external [momentum](../../../../momentum-split.md); an [on shell](../../../../on-shell.md) or massless limit must distinguish any [infrared divergence](../../../../infrared-divergence.md) from this [ultraviolet divergence](../../../../ultraviolet-divergence.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
