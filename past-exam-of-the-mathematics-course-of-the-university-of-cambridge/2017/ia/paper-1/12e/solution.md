<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

Let $L$ be the supremum of all [lower Darboux sums](../../../../../lower-darboux-sum.md) and $U$ the infimum of all [upper Darboux sums](../../../../../upper-darboux-sum.md). The assumed comparison of arbitrary lower and upper sums gives $L\leq U$. For the partition supplied for a given $\varepsilon$,

$$
0\leq U-L\leq S_{\mathcal D}(f)-s_{\mathcal D}(f)<\varepsilon.
$$

Since this holds for every positive $\varepsilon$, $U=L$. Thus the [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) gives

$$
\boxed{f\text{ is Riemann integrable}.}
$$

If $f$ is continuous on $[a,b]$, the [Heine-Cantor theorem](../../../../../heine-cantor-theorem.md) makes it uniformly continuous. Given $\varepsilon>0$, choose $\delta$ so that intervals of length below $\delta$ have oscillation below $\varepsilon/(b-a)$. A partition of mesh below $\delta$ then satisfies

$$
S_{\mathcal D}(f)-s_{\mathcal D}(f)<\varepsilon,
$$

proving that [Continuous functions are Riemann integrable](../../../../../continuous-functions-are-riemann-integrable.md).

For the function defined using $g$, choose $K$ with $|f|\leq K$. Given $\varepsilon>0$, choose $\delta>0$ so small that $2K\delta<\varepsilon/2$. On $[\delta,1]$, the function $g$ is continuous and therefore has a partition whose upper-minus-lower sum is below $\varepsilon/2$. Adding the interval $[0,\delta]$ contributes at most $2K\delta$, regardless of the value $f(0)=\lambda$. Hence the full Darboux-sum difference is below $\varepsilon$, and

$$
\boxed{f\text{ is Riemann integrable for every }\lambda\in\mathbb R}.
$$

Finally, for any partition $a=x_0<\cdots<x_n=b$, the [mean value theorem](../../../../../mean-value-theorem.md) supplies $\xi_i\in(x_{i-1},x_i)$ such that

$$
f(x_i)-f(x_{i-1})=f'(\xi_i)(x_i-x_{i-1}).
$$

Summing telescopes to

$$
f(b)-f(a)=\sum_{i=1}^nf'(\xi_i)(x_i-x_{i-1}),
$$

a [Riemann sum](../../../../../riemann-sum.md) for the Riemann-integrable function $f'$. Equivalently, every lower derivative sum is at most this telescoping value and every upper derivative sum is at least it. Taking the common [upper and lower Darboux integrals](../../../../../upper-and-lower-darboux-integrals.md) proves the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) conclusion

$$
\boxed{\int_a^bf'(x)\,dx=f(b)-f(a)}.
$$

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
