<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For any $v\in H^1(\Omega)$, expand $J(u+\epsilon v)$ in $\epsilon$. Its linear term must vanish at a minimizer, giving

$$
\int_\Omega(\nabla u\cdot\nabla v+uv)=\int_\Omega fv.
$$

Thus the required functionals are

$$
\boxed{a(u,v)=\int_\Omega(\nabla u\cdot\nabla v+uv),\qquad
\ell(v)=\int_\Omega fv.}
$$

The form is continuous, symmetric, and [coercive](../../../../../coercive-bilinear-form.md), with $a(v,v)=\|v\|_{H^1}^2$. Conversely, this weak equation implies $J(u+w)=J(u)+\frac12a(w,w)$, so its unique solution is indeed the global minimizer.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
