<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $P=-F>0$. With $G=0$, the [Euler elastica](../../../../euler-elastica.md) equation is $EI\theta''+P\sin\theta=0$. [Linearization](../../../../linearization.md) about the straight configuration gives $EI\theta''+P\theta=0$. Under the [boundary conditions](../../../../boundary-condition.md) explicitly stated, $\theta(0)=\theta(L)=0$, a nonzero solution requires

$$
\boxed{P_n=EI\left(\frac{n\pi}{L}\right)^2,\qquad
\theta_n(s)=C\sin\frac{n\pi s}{L},\qquad n=1,2,\ldots.}
$$

Thus **with only the stated [boundary conditions](../../../../boundary-condition.md)**, the first critical compressive force is $\boxed{F_c=-\pi^2EI/L^2}$. The corresponding linear transverse [displacement field](../../../../displacement-field-mechanics.md), with $y(0)=0$, is

$$
y_n(s)=\frac{CL}{n\pi}\left(1-\cos\frac{n\pi s}{L}\right),
$$

and $x(s)=s$ to first order. These are the successive small-amplitude [buckling](../../../../buckling.md) modes. The nonlinear branches retain the [simple pendulum](../../../../simple-pendulum-split.md) equation; if the angular amplitude is $\theta_m$ and $m=\sin(\theta_m/2)$, fitting $n$ half-periods into the rod gives $P=4EI n^2K(m)^2/L^2$, which tends to $P_n$ as $m\downarrow0$. Here $K$ is the [complete elliptic integral of the first kind](../../../../complete-elliptic-integral-of-the-first-kind.md), with $m$ its modulus, not its squared parameter.

**[Endpoint position compatibility for the Euler elastica](../../../../endpoint-position-compatibility-for-the-euler-elastica.md) adds a condition when fully fixed clamps have equal transverse height.** If the word “clamped” also imposes $y(L)=y(0)$, then $\int_0^L\theta_n\,ds=0$. With $G=0$, this retains only even $n=2j$, yielding

$$
\boxed{P_j=4j^2\pi^2EI/L^2,\qquad P_{\rm first}=4\pi^2EI/L^2.}
$$

The same exclusion is exact on the nonlinear branches: integrating the elastica equation gives $P\int\sin\theta\,ds=-EI[\theta'(L)-\theta'(0)]$, and an odd number of half-periods reverses the nonzero endpoint slope. Hence odd $n$ changes the endpoint height. The conventional fixed-clamp first [Euler buckling](../../../../euler-s-critical-load.md) load is the second boxed value, whereas the source's explicitly listed [boundary conditions](../../../../boundary-condition.md) alone give the first. Additional clamped modes with a nonzero transverse reaction require releasing the imposed $G=0$. Load-controlled buckling also permits axial shortening; an exactly inextensible rod whose endpoint separation is fixed equal to its full length has no room to buckle.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
