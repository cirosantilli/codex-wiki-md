<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

For an integrand $I(y,y')$ with no explicit $x$ dependence, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $I_y-d(I_{y'})/dx=0$. Differentiate the proposed first integral:

$$
\frac d{dx}(I-y'I_{y'})=I_yy'+I_{y'}y''-y''I_{y'}-y'\frac d{dx}I_{y'}
=y'\left(I_y-\frac d{dx}I_{y'}\right)=0.
$$

Thus **$I-y'I_{y'}$ is constant along an extremal**, the [Beltrami identity](../../../../../beltrami-identity.md).

For the optical path the [Fermat principle](../../../../../fermat-principle.md) uses the travel-time integrand $I=e^{-\lambda y}\sqrt{1+y'^2}$, in the stated speed units. Its first integral is

$$
\frac{e^{-\lambda y}}{\sqrt{1+y'^2}}=k>0,\qquad
y'^2=k^{-2}e^{-2\lambda y}-1.
$$

Set $u=ke^{\lambda y}$. Then $u'^2=\lambda^2(1-u^2)$, and integration gives $u=\cos[\lambda(x-x_0)]$ on a positive arch. The symmetric endpoint conditions require $x_0=0$ and $k=\cos\lambda a$. For $\lambda>0$ and $0<\lambda a<\pi/2$, the resulting [ray in an exponential-speed medium](../../../../../ray-in-an-exponential-speed-medium.md) is

$$
\boxed{y(x)=\frac1\lambda\log\left(\frac{\cos\lambda x}{\cos\lambda a}\right).}
$$

It is above zero inside the endpoints. Substitution also verifies the Euler-Lagrange equation $y''=-\lambda(1+y'^2)$, so the first-integral construction does not accidentally select a spurious constant-height path.

<a id="18d/image-stationary-light-rays-in-an-exponential-speed-medium-including-a-near-critical-arch"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3-exponential-ray.png)

**[Figure 1](#18d/image-stationary-light-rays-in-an-exponential-speed-medium-including-a-near-critical-arch). Stationary light rays in an exponential-speed medium, including a near-critical arch**.

Here $y'=-\tan\lambda x$. For $\lambda a$ close to $\pi/2$, the endpoint slopes are steep and the central height $-\lambda^{-1}\log\cos\lambda a$ is large. The travel time evaluates directly to

$$
\boxed{\mathcal T=\int_{-a}^a e^{-\lambda y}\sqrt{1+y'^2}\,dx
=\cos\lambda a\int_{-a}^a\sec^2\lambda x\,dx
=\frac2\lambda\sin\lambda a.}
$$

It tends to $2/\lambda$ as the arch height diverges. Positive $\lambda$ is the increasing-speed interpretation needed for a ray arching into $y>0$; for $\lambda<0$ the same algebraic expression bends below that region and is not an admissible interior path. At zero $\lambda$ the limiting straight boundary path has travel time $2a$.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
