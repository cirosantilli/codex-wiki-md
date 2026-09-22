# Coercive bilinear form

↑ **Parent:** [Bilinear form](bilinear-form-split.md)

A real [bilinear form](bilinear-form-split.md) $B$ on a [normed vector space](normed-vector-space-split.md) $X$ is coercive when there is one constant $\alpha>0$ such that

$$
B(v,v)\geq\alpha\|v\|^2\qquad(v\in X).
$$

The lower bound uniformly controls every direction in the chosen [norm](norm.md). Unlike the upper bound defining a [bounded bilinear form](bounded-bilinear-form.md), it forces positive diagonal values at every nonzero [vector](vector.md). No symmetry is assumed. For complex [Hilbert spaces](hilbert-space-split.md), the usual analogue uses a [sesquilinear form](sesquilinear-form.md) and $\operatorname{Re}B(v,v)\geq\alpha\|v\|^2$; it is not the same assertion for a complex [bilinear form](bilinear-form-split.md).

A concrete bounded and coercive example on $\mathbb R^2$, with the [Euclidean norm](euclidean-norm.md), is

$$
A=\begin{pmatrix}2&1\\-1&3\end{pmatrix},\qquad B(u,v)=u^TAv.
$$

Its [quadratic form](quadratic-form-split.md) is

$$
q(x,y)=B((x,y),(x,y))=2x^2+3y^2\geq2(x^2+y^2).
$$

The best lower constant is $\alpha=2$, attained at $(1,0)$. Nevertheless, $B(e_1,e_2)=1$ and $B(e_2,e_1)=-1$, so coercivity does not imply a [symmetric bilinear form](symmetric-bilinear-form.md). The [symmetric part of a matrix](symmetric-part-of-a-matrix.md) $S=(A+A^T)/2=\operatorname{diag}(2,3)$ determines $q$, while the [skew-symmetric matrix](skew-symmetric-matrix.md) part changes mixed pairings without changing $q$. This is the [symmetric and alternating parts of a bilinear form](symmetric-and-alternating-parts-of-a-bilinear-form.md) decomposition.[Theorem 1.7 and equation (1.3): symmetric and alternating parts](bilinear-forms-by-keith-conrad.md)

For the upper constant, direct multiplication gives $A^TA=\begin{pmatrix}5&-1\\-1&10\end{pmatrix}$. Its [eigenvalues](eigenvalue.md) are $(15\pm\sqrt{29})/2$, so the optimal upper constant, the [spectral norm](matrix-2-norm.md), is $C=\sqrt{(15+\sqrt{29})/2}$. The two constants answer different questions: how large a mixed pairing can be, and how small a self-pairing can be relative to squared [norm](norm.md).

<a id="image-bounded-saddle-and-flat-direction-quadratic-forms-contrasted-with-a-uniformly-coercive-bowl"></a>
![](bilinear-form-coercivity-energy-landscapes.png)

**[Figure 5](#image-bounded-saddle-and-flat-direction-quadratic-forms-contrasted-with-a-uniformly-coercive-bowl). Bounded saddle and flat-direction quadratic forms contrasted with a uniformly coercive bowl**.

The plotted [quadratic forms](quadratic-form-split.md) show the mechanism: $x^2-y^2$ descends in one direction, $x^2$ leaves one direction uncontrolled, and $2x^2+3y^2$ controls both. These are self-pairings; their [level sets](level-set.md) cannot reveal the [skew-symmetric matrix](skew-symmetric-matrix.md) part. Calling $q$ a quadratic energy here refers to this diagnostic quantity, not to a claim that a nonsymmetric equation comes from minimizing an [energy functional](energy-functional.md).

On a real [finite-dimensional vector space](finite-dimensional-vector-space.md) with any [norm](norm.md), strict positivity $B(v,v)>0$ for every nonzero $v$ does imply coercivity. Indeed the [quadratic form](quadratic-form-split.md) is [continuous](continuous-function.md), and its positive minimum on the [compact](compact-space.md) [unit sphere](unit-sphere.md) supplies $\alpha$. If $B$ is also a [symmetric bilinear form](symmetric-bilinear-form.md), this is [positive definiteness](positive-definiteness.md). For general $B$, it is the [symmetric and alternating parts of a bilinear form](symmetric-and-alternating-parts-of-a-bilinear-form.md) decomposition that isolates the positive part. Switching between [equivalent norms](equivalent-norms.md) preserves coercivity, but usually changes its constant.

The [infinite-dimensional vector space](infinite-dimensional-vector-space.md) distinction is explicit on the real [l2 sequence space](l2-sequence-space.md):

$$
B(u,v)=\sum_{n=1}^{\infty}\frac{u_nv_n}{n}.
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives boundedness with $C=1$, and $B(v,v)>0$ for every nonzero [vector](vector.md). But $B(e_n,e_n)=1/n$ with $\|e_n\|_2=1$, so no positive $\alpha$ works. On the [span](linear-span.md) of $e_1,\ldots,e_N$, the best lower constant is $1/N$: each finite restriction is coercive, but the control disappears as $N$ grows. Strict positivity is therefore weaker than a uniform lower bound.

The practical payoff is a stability estimate for a [weak formulation](weak-formulation.md). Assume $H$ is a real [Hilbert space](hilbert-space-split.md), $B:H\times H\to\mathbb R$ is both a [bounded bilinear form](bounded-bilinear-form.md) and a [coercive bilinear form](coercive-bilinear-form.md), and the load $\ell\in H'$ is a [bounded linear functional](continuous-linear-functional.md). The [Lax-Milgram theorem](lax-milgram-theorem.md) gives a unique $u\in H$ satisfying $B(u,v)=\ell(v)$ for all $v\in H$, including nonsymmetric $B$.[§2.2, Theorem 2.7, pp. 20–21, equation (2.9): hypotheses, unique solvability and load bound](introduction-to-finite-element-methods-by-christian-clason.md) The [dual norm](dual-norm.md) $\|\ell\|_{H'}=\sup_{v\ne0}|\ell(v)|/\|v\|$ measures load size. Testing with $v=u$ gives the short [energy estimate](energy-estimate.md)

$$
\alpha\|u\|^2\leq B(u,u)=\ell(u)\leq\|\ell\|_{H'}\|u\|,\qquad
\|u\|\leq\frac{\|\ell\|_{H'}}{\alpha}.
$$

For $u=0$ the bound holds directly; otherwise divide by $\|u\|$. Subtracting the equations for two loads and using the same argument gives $\|u_1-u_2\|\leq\|\ell_1-\ell_2\|_{H'}/\alpha$. Thus a positive lower constant limits the response to load errors. The upper bound and [completeness](completeness.md) of the [Hilbert space](hilbert-space-split.md) enter the existence theorem; the estimate itself uses the lower bound and the load's [dual norm](dual-norm.md).

For the displayed [matrix](matrix.md) $A$, take $\ell(v)=f^Tv$. Then $B(u,v)=\ell(v)$ for every $v$ means $A^Tu=f$, not $Au=f$, with this ordering of the [bilinear form](bilinear-form-split.md). Since $\det A=7$,

$$
u=\frac17\begin{pmatrix}3&1\\-1&2\end{pmatrix}f,\qquad
\|u\|_2\leq\frac12\|f\|_2.
$$

For $f=t(1,0)^T$, the exact response is $u=t(3,-1)^T/7$ and $\|u\|_2=\sqrt{10}|t|/7<|t|/2$. For $f=t(0,1)^T$, it is $u=t(1,2)^T/7$, with [norm](norm.md) $\sqrt5|t|/7$. The actual maximal amplification is the [operator norm](operator-norm.md) $\|(A^T)^{-1}\|_2=\sqrt{2/(15-\sqrt{29})}<1/2$: the coercivity estimate is valid but need not be sharp for a nonsymmetric [bilinear form](bilinear-form-split.md).

<a id="image-solutions-for-unit-loads-lie-inside-the-coercivity-bound-and-response-grows-at-most-linearly-with-load-norm"></a>
![](coercive-bilinear-form-load-response-bound.png)

**[Figure 6](#image-solutions-for-unit-loads-lie-inside-the-coercivity-bound-and-response-grows-at-most-linearly-with-load-norm). Solutions for unit loads lie inside the coercivity bound, and response grows at most linearly with load norm**.

## ↑ Ancestors (6)

1. [Bilinear form](bilinear-form-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Bounded bilinear form](bounded-bilinear-form.md)
- [Clamped biharmonic problem](clamped-biharmonic-problem.md)
- [Coercive bilinear form](coercive-bilinear-form.md)
- [Coercive variable-coefficient Dirichlet form](coercive-variable-coefficient-dirichlet-form.md)
- [Constant-drift massive-Laplacian Dirichlet problem](constant-drift-massive-laplacian-dirichlet-problem.md)
- [Finite element mesh](finite-element-mesh.md)
- [Finite element method](finite-element-method-split.md)
- [Finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md)
- [Galerkin orthogonality](galerkin-orthogonality.md)
- [Lax-Milgram theorem](lax-milgram-theorem.md)
- [Mixed-boundary Airy energy principle](mixed-boundary-airy-energy-principle.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-12/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/1/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/23h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/23h/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-105/2/c/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-105/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-105/2/e/solution.md)
- [Quadratic variational principle for a symmetric positive operator](quadratic-variational-principle-for-a-symmetric-positive-operator.md)
- [Ritz-Galerkin equivalence for a symmetric coercive form](ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md)
- [Stiffness matrix](stiffness-matrix.md)
- [Strict positivity without coercivity can fail variational solvability](strict-positivity-without-coercivity-can-fail-variational-solvability.md)
- [Symmetry and coercivity in quadratic energy minimization](symmetry-and-coercivity-in-quadratic-energy-minimization.md)
- [Variational problem](variational-problem.md)
