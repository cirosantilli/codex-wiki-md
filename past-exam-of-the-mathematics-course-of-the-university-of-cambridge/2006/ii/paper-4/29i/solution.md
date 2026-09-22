<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

Solve the bank equation first:

$$
x(T)=W-\int_0^T e^{r(T-t)}u(t)dt,\qquad
W=e^{rT}x(0)+\frac A r(e^{rT}-1)>0.
$$

For $\mu>0$ the objective separates into pointwise strictly concave functions of positive $u$. Their derivative is $e^{-\beta t}/u-\mu e^{-\beta T}e^{r(T-t)}$. Setting it to zero gives the unique optimum

$$
\boxed{u^*(t;\mu)=\mu^{-1}e^{(\beta-r)(T-t)}}.
$$

Let $B=\int_0^T e^{\beta s}ds$, equal to $(e^{\beta T}-1)/\beta$ when $\beta\ne0$ and $T$ otherwise. Then $x^*(T;\mu)=W-B/\mu$ is strictly increasing from negative infinity to $W$ as $\mu$ increases from zero to infinity. Consequently

$$
\boxed{\mu^*=B/W}
$$

is the unique positive multiplier with zero terminal balance.

For the constrained problem with no terminal reward, $x(T)\ge0$ is exactly the weighted spending budget $\int e^{r(T-t)}u(t)dt\le W$. The candidate $u^*(\cdot;\mu^*)$ spends that budget exactly. Concavity gives $\log u-\log u^*\le(u-u^*)/u^*$. Since $e^{-\beta t}/u^*=\mu^*e^{-\beta T}e^{r(T-t)}$, integrating this inequality makes the [utility function](../../../../../utility-function-split.md) difference nonpositive for every feasible control. This proves the requested optimality of the [logarithmic spending with a terminal multiplier](../../../../../logarithmic-spending-with-a-terminal-multiplier.md) solution directly, including uniqueness up to changes on measure-zero sets.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
