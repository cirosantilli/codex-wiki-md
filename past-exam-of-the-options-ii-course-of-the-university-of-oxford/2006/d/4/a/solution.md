<h1 id="d/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We first prove the differentiation theorem. Fix $t\in(0,b)$ and take nonzero $h\to0$ with $t+h\in(0,b)$. The [measurable](../../../../../measurability.md) difference quotients

$$
q_h(x)=\frac{f(x,t+h)-f(x,t)}h
$$

converge pointwise to $f_t(x,t)$. The [mean value theorem](../../../../../mean-value-theorem.md) and the assumed derivative bound give $|q_h(x)|\leq g(x)$. In particular $f_t(\cdot,t)$ is [measurable](../../../../../measurability.md) as a limit of quotients along a sequence, and its bound by $g$ proves integrability. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), in its parameter-limit form, says that pointwise convergence with a common integrable bound permits convergence of the integrals. Applying it yields

$$
\boxed{\frac d{dt}\int_0^\infty f(x,t)dx
=\lim_{h\to0}\int_0^\infty q_h(x)dx
=\int_0^\infty f_t(x,t)dx.}
$$

The parameter-limit statement follows from the ordinary sequential theorem by applying it to every sequence of nonzero $h$ tending to zero.

For the specific function, $|f(x,t)|\leq e^{-x^2}$, which is integrable by the allowed fact. It is differentiable in $t$, with

$$
f_t(x,t)=-2xe^{-x^2}\sin(2xt),\qquad
|f_t(x,t)|\leq2xe^{-x^2}.
$$

The last majorant has integral one on $[0,\infty)$, using the substitution $u=x^2$. All three hypotheses therefore hold. The indicator of the parameter domain is one at every point under consideration and does not affect this derivative.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [D](../../../d.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
