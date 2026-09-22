<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Sobolev space](../../../../sobolev-space-split.md) $H^1(b,c)$ consists of $L^2$ functions with a weak first derivative in $L^2$, with norm

$$
\|v\|_{H^1}^2=\int_b^c(|v|^2+|v'|^2)\,dx.
$$

In one dimension these functions have absolutely continuous representatives and well-defined endpoint [Sobolev traces](../../../../trace-operator.md). Put

$$
V=\{v\in H^1(b,c):v(b)=0\}.
$$

This is a closed subspace, hence a Hilbert space. Both trial and test functions belong to $V$; one does not impose a derivative boundary condition in this space.

Integrate the differential equation against $v\in V$:

$$
\int_b^cfv=\int_b^ce^xu'v'\,dx-e^cu'(c)v(c).
$$

The printed condition uses the ordinary derivative, $u'(c)=-u(c)$, so the weak form is

$$
\boxed{a(u,v)=\int_b^ce^xu'v'\,dx+e^cu(c)v(c),\qquad
\ell(v)=\int_b^cfv\,dx.}
$$

Seek $u\in V$ with $a(u,v)=\ell(v)$ for all $v\in V$. The coefficient $e^c$ in the endpoint term must be retained: replacing the ordinary derivative with the conormal flux would change the boundary problem.

Let $L=c-b$. The [Poincaré inequality](../../../../poincare-inequality.md) on $V$ can be stated as $\|v\|_{L^2}\leq L\|v'\|_{L^2}$. Also $|v(c)|\leq\sqrt L\|v'\|_{L^2}$. Consequently

$$
a(v,v)\geq e^b\|v'\|_{L^2}^2
\geq\alpha\|v\|_{H^1}^2,\qquad
\alpha=\frac{e^b}{1+L^2}>0,
$$

proving coercivity. By [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) and the trace bound,

$$
|a(u,v)|\leq e^c(1+L)\|u\|_{H^1}\|v\|_{H^1}.
$$

Thus continuity holds with $M=e^c(1+L)$. The load is continuous if $f\in L^2$, and the [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) gives a unique weak solution.

Choose a finite-dimensional conforming subspace $V_h\subset V$, such as continuous piecewise linear functions vanishing at $b$, and solve $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$. Subtracting the weak equations gives [Galerkin orthogonality](../../../../galerkin-orthogonality.md) $a(u-u_h,v_h)=0$.

[Céa's lemma](../../../../cea-s-lemma.md) states, for a continuous coercive bilinear form with constants $M,\alpha$ on a Hilbert space,

$$
\boxed{\|u-u_h\|_{H^1}\leq\frac M\alpha
\inf_{v_h\in V_h}\|u-v_h\|_{H^1}.}
$$

To prove it, put $e=u-u_h$ and use orthogonality to write $a(e,e)=a(e,u-v_h)$ for any $v_h\in V_h$. Coercivity and continuity give $\alpha\|e\|^2\leq M\|e\|\|u-v_h\|$. If $e=0$ the claim is immediate; otherwise cancel its norm and take the infimum. Any approximation theorem making the infimum tend to zero under mesh refinement therefore gives strong convergence $u_h\to u$ in $H^1$.

Finally, $a$ is symmetric and positive definite on $V$. It is an inner product, so $\|v\|_a=\sqrt{a(v,v)}$ is an [energy norm](../../../../energy-norm.md) on all of $V$: homogeneity and definiteness are immediate, and [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) for this inner product gives the triangle inequality. No smaller space is required. In this norm the continuity and coercivity constants are one. More precisely, [Galerkin orthogonality](../../../../galerkin-orthogonality.md) gives

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2,
$$

so

$$
\boxed{\|u-u_h\|_a=\min_{v_h\in V_h}\|u-v_h\|_a.}
$$

The finite element solution is the exact best energy-norm approximation.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../split.md)
5. [Approximation theory and finite element methods course of the University of Oxford](../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
