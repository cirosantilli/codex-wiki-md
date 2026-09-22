<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

For the regular Sturm-Liouville setting assume $p$ is positive and continuously differentiable, $q,w$ are [continuous](../../../../continuous-function.md), and $w>0$. Apply a multiplier to $J[y]-\lambda(\int_a^bwy^2-1)$. Its [first variation](../../../../first-variation.md), divided by two, is

$$
[p y'\eta]_a^b-\int_a^b[(py')'+qy+\lambda wy]\eta\,dx.
$$

Endpoint-vanishing variations and the allowed fundamental lemma give

$$
\boxed{-(py')'-qy=\lambda wy}.
$$

If an endpoint value is free, its [variation](../../../../variation.md) is arbitrary, giving the natural condition $py'=0$ at that endpoint. At a prescribed endpoint value the [variation](../../../../variation.md) vanishes there, so no additional natural condition is imposed.

For eigenfunctions $u,v$ with different eigenvalues, multiply their equations by $v,u$ and subtract after integration. The resulting boundary expression $[p(uv'-u'v)]_a^b$ vanishes under common homogeneous Dirichlet or common natural boundary conditions. Hence $(\lambda_u-\lambda_v)\int_a^bwuv=0$, proving weighted [orthogonality](../../../../orthogonal-vectors.md).

For the final Dirichlet problem the normalized stationary modes are

$$
\boxed{y_k(x)=\pm\sqrt2\sin(k\pi x),\qquad\lambda_k=k^2\pi^2-1,\quad k\geq1}.
$$

Solving $y''+(\lambda+1)y=0$ with both endpoint values zero gives these and excludes nonpositive $\lambda+1$. Distinct sine modes have zero integral product on $[0,1]$. Their Dirichlet values also make the same boundary expression vanish, which explains [orthogonality](../../../../orthogonal-vectors.md) even though their endpoint derivatives do not obey the natural conditions.

For global minimality, the Fourier sine expansion of an endpoint-vanishing [function](../../../../function-split.md) and Parseval's identities give $\int y'^2=\sum k^2\pi^2a_k^2\geq\pi^2\sum a_k^2=\pi^2\int y^2$. Equality holds exactly in the first sine eigenspace. Therefore

$$
\boxed{\min J=\pi^2-1=\lambda_1,\qquad y=\pm\sqrt2\sin(\pi x)}.
$$

Distinct modes are [orthogonal](../../../../orthogonal-vectors.md); the two sign choices of the same minimum are not [orthogonal](../../../../orthogonal-vectors.md) to each other. This distinguishes the family of stationary modes from the two representatives of the minimizing eigenspace in the question's wording.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2008 printed variant](../../../2008-printed-variant-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
