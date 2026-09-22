<h1 id="aubin-nitsche-duality-argument">Aubin–Nitsche duality argument</h1>

↑ **Parent:** [Céa's lemma](cea-s-lemma.md)

For a symmetric elliptic variational problem with [Galerkin orthogonality](galerkin-orthogonality.md), let $e=u-u_h$ and solve the dual problem $a(v,z)=(e,v)_{L^2}$ for every $v\in H_0^1(\Omega)$. If [elliptic regularity](elliptic-regularity.md) gives $\|z\|_{H^2}\leq C\|e\|_{L^2}$, then a [finite element interpolation estimate](finite-element-interpolation-estimate.md) gives

$$
\|e\|_{L^2}^2=a(e,z-I_hz)
\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Thus $\|e\|_{L^2}\leq Ch\|e\|_{H^1}$. Combining this with the [Céa lemma](cea-s-lemma.md) and an $O(h)$ [energy norm](energy-norm.md) error gives an $O(h^2)$ [L2 norm](l2-norm.md) error. The additional order depends on the dual regularity assumption, which can fail on unsuitable domains.

**Table of contents**

- [Explicit one-dimensional dual residual bound in L2](explicit-one-dimensional-dual-residual-bound-in-l2.md)

## ↑ Ancestors (8)

1. [Céa's lemma](cea-s-lemma.md)
2. [Galerkin orthogonality](galerkin-orthogonality.md)
3. [Finite element method](finite-element-method-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2010/b/5/solution.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/7/solution.md)
- [Reaction-diffusion regularity from Laplacian regularity](reaction-diffusion-regularity-from-laplacian-regularity.md)
