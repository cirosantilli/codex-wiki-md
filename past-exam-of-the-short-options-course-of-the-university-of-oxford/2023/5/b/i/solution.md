<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For real $p>0$, substitute $t=px$ in the [Laplace transform](../../../../../laplace-transform.md):

$$
\int_0^\infty x^{a-1}e^{-px}\,dx=p^{-a}\int_0^\infty t^{a-1}e^{-t}\,dt=\boxed{\Gamma(a)p^{-a}}.
$$

The [Gamma function](../../../../../gamma-function.md) integral is finite because $a>0$. For complex $p$, absolute convergence holds exactly when $\operatorname{Re}p>0$: the modulus of the integrand is $x^{a-1}e^{-(\operatorname{Re}p)x}$. On this half-plane the same answer holds with the branch $p^{-a}=\exp(-a\operatorname{Log}p)$ whose logarithm is real on the positive axis, by holomorphic continuation of the two sides.

If “exists” permits conditionally convergent ordinary improper integrals, there are additional boundary points when $0<a<1$: for $p=i\omega\ne0$, the [Dirichlet test](../../../../../dirichlet-test.md) gives convergence, with value $\Gamma(a)|\omega|^{-a}e^{-i\operatorname{sgn}(\omega)\pi a/2}$. For $a\geq1$ these boundary integrals do not converge in that sense. At $p=0$, and for $\operatorname{Re}p<0$, the integral diverges. Thus $\operatorname{Re}p>0$ is the [region of absolute convergence of a Laplace transform](../../../../../region-of-absolute-convergence-of-a-laplace-transform.md), with the stated conditional boundary qualification.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
