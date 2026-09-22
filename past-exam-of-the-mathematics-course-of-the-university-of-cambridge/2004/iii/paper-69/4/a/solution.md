<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V$ be a real [Hilbert space](../../../../../../hilbert-space-split.md), $a:V\times V\to\mathbb R$ a [bounded bilinear form](../../../../../../bounded-bilinear-form.md), and $\ell\in V'$ a [bounded linear functional](../../../../../../continuous-linear-functional.md). Assume constants $C<\infty$, $\alpha>0$ satisfy

$$
|a(v,w)|\le C\|v\|_V\|w\|_V,\qquad a(v,v)\ge\alpha\|v\|_V^2\qquad(v,w\in V).
$$

The second hypothesis says that $a$ is a [coercive bilinear form](../../../../../../coercive-bilinear-form.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) then supplies a unique [weak solution](../../../../../../weak-solution.md) $u\in V$ with $a(u,v)=\ell(v)$ for every $v\in V$, and $\|u\|_V\le\|\ell\|_{V'}/\alpha$.

For a finite-dimensional trial [linear subspace](../../../../../../vector-subspace.md) $V_h\subset V$, the same boundedness and coercivity constants apply to the restricted form. Since a [finite-dimensional subspace is closed](../../../../../../finite-dimensional-subspace-is-closed.md), $V_h$ is itself a [Hilbert space](../../../../../../hilbert-space-split.md). Thus there is a unique [Galerkin method](../../../../../../galerkin-method.md) solution $u_h\in V_h$ satisfying $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$. The [Galerkin orthogonality](../../../../../../galerkin-orthogonality.md) $a(u-u_h,v_h)=0$ gives the [Céa lemma](../../../../../../cea-s-lemma.md):

$$
\boxed{\|u-u_h\|_V\le\frac C\alpha\inf_{v_h\in V_h}\|u-v_h\|_V}.
$$

In particular, approximation by the trial spaces implies [numerical convergence](../../../../../../convergence-of-a-numerical-method.md). For a complex [Hilbert space](../../../../../../hilbert-space-split.md), replace bilinearity by a [sesquilinear form](../../../../../../sesquilinear-form.md), take $\ell$ antilinear in the test variable, and require $\operatorname{Re}a(v,v)\ge\alpha\|v\|_V^2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
