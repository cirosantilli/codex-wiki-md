<h1 id="b/7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Two interval Poincaré inequalities give $\|z-I_hz\|_{2,I_i}\leq h_i^2\|z''\|_{2,I_i}/\pi^2$: the error has zero endpoint values and its [derivative](../../../../../derivative.md) has zero mean. Apply [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on each interval and then to the sum:

$$
\left|\int_0^1(u-u_h)\psi\right|
\leq\frac1{\pi^2}\left(\sum_i h_i^4\|R(u_h)\|_{2,I_i}^2\right)^{1/2}\|z''\|_2
\leq\frac{e+1}{\pi^2}\eta_h\|\psi\|_2.
$$

Here $\eta_h^2=\sum_i h_i^4\|R(u_h)\|_{2,I_i}^2$. Taking $\psi=u-u_h$ and cancelling its [norm](../../../../../norm.md), unless it is zero already, yields

$$
\boxed{\|u-u_h\|_2\leq\frac{e+1}{\pi^2}\eta_h.}
$$

For adaptive refinement, solve the discrete problem, compute $\eta_i^2=h_i^4\|R(u_h)\|_{2,I_i}^2$, and stop when $(e+1)\eta_h/\pi^2\leq\mathrm{TOL}$. Otherwise mark intervals carrying a fixed positive fraction of $\eta_h^2$, bisect them, and repeat. Residual integration must be exact or have a certified upper bound if the stopping test is to certify the requested tolerance.

Use [residual adaptation with a uniform-refinement safeguard](../../../../../residual-adaptation-with-a-uniform-refinement-safeguard.md), for example global bisection every second refinement, to ensure eventual termination. Discrete energy stability gives $\|u_h\|_{H^1}\leq\|f\|_2$, so $\|R(u_h)\|_2\leq(1+e)\|f\|_2$ independently of the mesh. Thus $\eta_h\leq h_{\max}^2(1+e)\|f\|_2$ tends to zero under the safeguard. Other iterations concentrate work where the residual is large.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
