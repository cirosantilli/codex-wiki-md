<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For independent available acceptors at equal distance, the [multiple-acceptor FRET efficiency](../../../../multiple-acceptor-fret-efficiency.md) follows by adding the $n$ parallel exit rates. Each contributes the same rate $k_T$, so the total rate is $nk_T$, rather than $n$ times the single-pair transfer [probability](../../../../probability.md). Hence

$$
E_n=\frac{nk_T}{k_D+nk_T},\qquad
\frac{k_T}{k_D}=\frac{E}{1-E},
\qquad\boxed{E_n=\frac{nE}{1+(n-1)E}.}
$$

Equivalently, $E_n=n/[n+(R/R_0)^6]$. Inverting gives

$$
\boxed{R=R_0\left[\frac{n(1-E_n)}{E_n}\right]^{1/6}.}
$$

With $n=3$ and $E_n=0.75$, the bracket is exactly one and $R=R_0=6.5$ nm. Each isolated pair would have efficiency $1/2$; the three transfer rates together give $3/(1+3)=3/4$. Multiplying $1/2$ by three would violate the [probability](../../../../probability.md) bound and is not a valid calculation.

This model assumes one donor excitation, identical pairwise transfer rates, no coherent coupling between acceptors, no acceptor saturation and no change in donor photophysics or orientation on adding labels. Different separations instead require summing $k_{T,j}$ individually. Acceptor-to-acceptor transfer can alter which acceptor emits; it does not automatically change the donor's first-transfer [probability](../../../../probability.md) when the donor exit rates remain those specified.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
