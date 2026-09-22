<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the zero initial displacement and velocity given in the PDF. The characteristic roots of the homogeneous equation are $-1\pm i\mu$. Its [causal Green function of a damped oscillator](../../../../../../causal-green-function-of-a-damped-oscillator.md) is

$$
G(t)=H(t)\frac{e^{-t}\sin(\mu t)}{\mu},
$$

where $H$ is the [Heaviside step function](../../../../../../heaviside-step-function.md). The positive-time kernel has $G(0+)=0$ and $G'(0+)=1$, so its [derivative](../../../../../../derivative.md) jump generates a unit impulse. The zero-data forced solution is consequently the causal [convolution](../../../../../../convolution.md)

$$
\boxed{x(t)=\frac1\mu\int_0^te^{-(t-s)}\sin[\mu(t-s)]g(s)\,ds,\qquad t\geq0.}
$$

Differentiating once gives $x'(0)=0$; differentiating twice supplies the endpoint term $g(t)$ and verifies the differential equation. No homogeneous transient is required with these initial data.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
