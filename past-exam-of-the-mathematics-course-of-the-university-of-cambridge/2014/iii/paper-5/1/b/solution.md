<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consider the [flat function](../../../../../../flat-function.md)

$$
f(x)=\begin{cases}e^{-1/x^2},&x\ne0,\\0,&x=0.\end{cases}
$$

Away from zero every [derivative](../../../../../../derivative.md) has the form $P_n(1/x)e^{-1/x^2}$ for a [polynomial](../../../../../../polynomial-split.md) $P_n$: differentiating preserves this form. For every $m\geq0$,

$$
\lim_{x\to0}|x|^{-m}e^{-1/x^2}=0,
$$

because an [exponential function](../../../../../../exponential-function.md) decays faster than any power. Inductively, extend each displayed [derivative](../../../../../../derivative.md) by zero at zero. It is continuous there, and its difference quotient at zero also tends to zero by the same estimate with one extra power of $|x|^{-1}$. Thus each extension is the [derivative](../../../../../../derivative.md) of the preceding extension. This proves $f\in C^\infty(\mathbb R)$ and $f^{(n)}(0)=0$ for all $n$.

Its [Taylor series](../../../../../../taylor-series.md) at zero is identically zero, whereas $f(x)>0$ for every $x\ne0$. **It is [smooth](../../../../../../smooth-function.md) everywhere but not [real analytic](../../../../../../real-analytic-function.md) at zero.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
