<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the usual regularity assumptions, the [Leibniz integral rule](../../../../../leibniz-integral-rule.md) is

$$
\boxed{\frac d{dx}\int_{g(x)}^{f(x)}h(x,t)\,dt=h(x,f(x))f'(x)-h(x,g(x))g'(x)+\int_{g(x)}^{f(x)}h_x(x,t)\,dt.}
$$

There is a genuine domain problem in the following integral as printed in the PDF. Put

$$
q(t)=\frac{2t^4+1}{(t-2)(t^2+3)}.
$$

The point $t=2$ is a simple pole, with

$$
\lim_{t\to2}(t-2)q(t)=\frac{33}{7}\ne0.
$$

For every $x>4$, the lower endpoint $\sin(1/x)$ is less than $2$ and the upper endpoint $\sqrt x$ is greater than $2$. The interval therefore crosses the pole. Since $q(t)=33/[7(t-2)]+O(1)$ near $2$, the two one-sided [improper integrals](../../../../../improper-integral.md) diverge logarithmically, with opposite signs. Their divergences do not define an ordinary [integral](../../../../../integral-split.md). Consequently **the ordinary limit in the question is undefined as written**: its underlying integral has no finite value for any $x\geq4$.

A separately specified [Cauchy principal value](../../../../../cauchy-principal-value.md) does exist for $x>4$. Under that interpretation, [differentiating a principal-value integral across a fixed simple pole](../../../../../differentiating-a-principal-value-integral-across-a-fixed-simple-pole.md) gives

$$
\frac d{dx}\operatorname{PV}\int_{\sin(1/x)}^{\sqrt x}q(t)\,dt=\frac{q(\sqrt x)}{2\sqrt x}+\frac{\cos(1/x)}{x^2}q(\sin(1/x)).
$$

The first term is

$$
\frac{2x^2+1}{2\sqrt x(\sqrt x-2)(x+3)}\longrightarrow1,
$$

and the second tends to zero because $q$ is bounded near $t=0$. Thus the principal-value version has limit $\boxed{1}$. The two conclusions are distinct: this regularised answer requires the additional principal-value convention, which the printed question does not state.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
