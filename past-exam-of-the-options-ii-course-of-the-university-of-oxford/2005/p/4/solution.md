<h1 id="p/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A real [inner product](../../../../inner-product-split.md) is a bilinear symmetric form satisfying $(v,v)>0$ for every nonzero $v$, and $(0,0)=0$. Its [norm](../../../../norm.md) is $\|v\|=\sqrt{(v,v)}$. An [orthogonal polynomial](../../../../orthogonal-polynomial-split.md) family has nonzero members of exact degrees $0,1,\ldots,k$, with $(\phi_i,\phi_j)=0$ for different indices. Exact degree is part of this definition; merely belonging to the indicated [polynomial vector spaces](../../../../polynomial-vector-space.md) would not suffice.

Distinct degrees make $\phi_0,\ldots,\phi_{\ell-1}$ [linearly independent](../../../../linear-independence.md). There are $\ell$ of them in the $\ell$-dimensional space $\Pi_{\ell-1}$, so they form a [basis](../../../../basis.md). Any lower-degree [polynomial](../../../../polynomial-split.md) is their [linear combination](../../../../linear-combination.md), and bilinearity therefore gives $(\phi_\ell,p)=0$ for every $p\in\Pi_{\ell-1}$.

Use the orthogonal-projection characterization: $p_*$ is the [best approximation](../../../../best-approximation-in-a-normed-space.md) to $v$ in a finite-dimensional subspace $W$ exactly when $v-p_*$ is [orthogonal](../../../../orthogonal-vectors.md) to $W$. Here $v=\phi_\ell$ is already [orthogonal](../../../../orthogonal-vectors.md) to $W=\Pi_{\ell-1}$, so its unique [best approximation](../../../../best-approximation-in-a-normed-space.md) is zero. For $\ell\ge1$, $\phi_{\ell-1}$ is nonzero and therefore cannot be that [best approximation](../../../../best-approximation-in-a-normed-space.md). Directly,

$$
\|\phi_\ell-\phi_{\ell-1}\|^2
=\|\phi_\ell\|^2+\|\phi_{\ell-1}\|^2>\|\phi_\ell\|^2.
$$

For the specified weight, symmetry makes every odd moment vanish, while

$$
\int_{-1}^1|x|x^{2m}\,dx=2\int_0^1x^{2m+1}\,dx=\frac1{m+1}.
$$

Choose $\phi_0=1$ and $\phi_1=x$. A monic quadratic [orthogonal](../../../../orthogonal-vectors.md) to $x$ has no linear term by symmetry, and [orthogonality](../../../../orthogonal-vectors.md) to 1 requires $\int|x|(x^2-c)dx=1/2-c=0$. Thus a valid answer is

$$
\boxed{\phi_0=1,\qquad\phi_1=x,\qquad\phi_2=x^2-\tfrac12.}
$$

The weight vanishes only at one point, so a nonzero [polynomial](../../../../polynomial-split.md) has positive squared [norm](../../../../norm.md); the form is indeed positive definite on the [polynomial vector space](../../../../polynomial-vector-space.md). Nonzero rescalings of individual family members give equally valid unnormalized answers.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [P](../../p.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
