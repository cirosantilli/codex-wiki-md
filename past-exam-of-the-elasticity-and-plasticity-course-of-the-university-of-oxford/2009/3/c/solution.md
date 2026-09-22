<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Insert the two constitutive stresses into the radial component of the [Cauchy momentum equation](../../../../cauchy-momentum-equation.md). After collecting terms, $(\lambda+2\mu)(u_r''+u_r'/r-u_r/r^2)=0$, so $u_r=Ar+B/r$. Its stresses are

$$
\tau_{rr}=2(\lambda+\mu)A-2\mu B/r^2,\qquad\tau_{\theta\theta}=2(\lambda+\mu)A+2\mu B/r^2.
$$

The far pressure gives $A=-p_\infty/[2(\lambda+\mu)]$. At the tunnel wall, compressive bracing imposes $\tau_{rr}(a)=-P$, so $B=(P-p_\infty)a^2/(2\mu)$. Hence

$$
\boxed{\tau_{rr}=-p_\infty-\frac{a^2}{r^2}(P-p_\infty),\quad\tau_{\theta\theta}=-p_\infty+\frac{a^2}{r^2}(P-p_\infty),}
$$



$$
\boxed{u_r=-\frac{p_\infty r}{2(\lambda+\mu)}+\frac{(P-p_\infty)a^2}{2\mu r}.}
$$

With no shear and $\tau_{\theta\theta}=k\tau_{rr}$, divide the yield identity by the nonzero $\tau_{rr}^2$ to obtain $4k=(1+k)^2\cos^2\phi$. Solving its quadratic gives

$$
\boxed{k_+=\frac{1+\sin\phi}{1-\sin\phi},\qquad k_-=\frac{1-\sin\phi}{1+\sin\phi}.}
$$

To locate first yield, the [stress](../../../../stress.md)-circle center is the constant $-p_\infty$, while its radius is $|P-p_\infty|a^2/r^2$. The radius is maximal at $r=a$, so that is where it first meets the [friction](../../../../friction.md) envelope as the bracing departs from the hydrostatic value. At the wall $\tau_{rr}=-P$ and $\tau_{\theta\theta}=P-2p_\infty$; hence $k=(2p_\infty-P)/P$ and

$$
\boxed{P=\frac{2p_\infty}{1+k}.}
$$

For lowering bracing from $P=p_\infty$, the hoop [stress](../../../../stress.md) becomes more compressive, so $k=k_+>1$ and $\boxed{P_{\rm crit}=p_\infty(1-\sin\phi)}$. Increasing bracing instead selects $k_-$ and reaches the other threshold $p_\infty(1+\sin\phi)$. Stating the loading direction removes any ambiguity between the two reciprocal [stress](../../../../stress.md) ratios. These conclusions describe first yield of the elastic field, not the later plastic-zone solution.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
