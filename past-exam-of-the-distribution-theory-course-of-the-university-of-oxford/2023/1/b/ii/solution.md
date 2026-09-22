<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**No.** Consider the continuous even [function](../../../../../function-split.md)

$$
f(x)=\begin{cases}
0,&x=0,\\
1/\log(1/|x|),&0<|x|\leq e^{-1},\\
1,&|x|\geq e^{-1}.
\end{cases}
$$

The formulas agree at $|x|=e^{-1}$, and $f(x)\to0$ at zero. Part (i) defines its [even-weight principal-value distribution](../../../../../even-weight-principal-value-distribution.md). However,

$$
\boxed{\int_0^{e^{-1}}\frac{|f(x)|}{x}\,dx
=\int_1^\infty\frac{ds}{s}=\infty,\qquad s=\log(1/x).}
$$

If this were a [regular distribution](../../../../../regular-distribution.md) represented by $g\in L^1_{\mathrm{loc}}(\mathbb R)$, testing on either side of zero would force $g=f/x$ [almost everywhere](../../../../../almost-everywhere.md) there, by uniqueness of the [locally integrable function](../../../../../locally-integrable-function.md) representing a [regular distribution](../../../../../regular-distribution.md). Changing the value at zero cannot remove the displayed divergence, contradicting [local integrability](../../../../../locally-integrable-function.md) of $g$.

More generally, the exact condition is

$$
\boxed{\operatorname{pv}(f/x)\text{ is regular}\iff
\int_0^r\frac{|f(x)|}{x}\,dx<\infty\text{ for some }r>0.}
$$

Necessity is the preceding argument; sufficiency follows because $f/x$ is then a [locally integrable function](../../../../../locally-integrable-function.md) and its truncated integrals converge absolutely. The value $f(0)=0$ alone provides no such rate of decay.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
