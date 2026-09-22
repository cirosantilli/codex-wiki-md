<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $M=\|F'\|_\infty$. The sharper [energy estimate](../../../../../../../energy-estimate.md) uses the divergence structure of the [viscous scalar conservation law](../../../../../../../viscous-scalar-conservation-law.md). Multiply by $u$ and integrate over the line. With $G(s)=\int_0^s rF'(r)\,dr$,

$$
\int u\partial_xF(u)=\int\partial_xG(u)=0,
$$

because the decay makes $G(u)$ tend to zero at both ends. [Integration by parts](../../../../../../../integration-by-parts.md) in the diffusion term therefore gives

$$
\frac12\frac{d}{dt}\|u(t)\|_2^2+\varepsilon\|u_x(t)\|_2^2=0,
\qquad
\boxed{\|u(t)\|_2^2+2\varepsilon\int_0^t\|u_x(s)\|_2^2\,ds=\|u(0)\|_2^2.}
$$

**One may take $C_0=0$, uniformly in $\varepsilon$.** This does not require $F(0)=0$.

If a bound explicitly involving $M$ and $\varepsilon$ is desired, retaining the transport term and using the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) and the elementary inequality $ab\leq(a^2+b^2)/2$ gives

$$
M\|u\|_2\|u_x\|_2\leq\frac\varepsilon2\|u_x\|_2^2+\frac{M^2}{2\varepsilon}\|u\|_2^2.
$$

The [Gronwall inequality](../../../../../../../gronwall-inequality.md) then gives the valid but weaker choice $C_0=M^2/\varepsilon$. The exact cancellation explains why its divergence is unnecessary.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
