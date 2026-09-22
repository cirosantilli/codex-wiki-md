<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

Associate to $Q$ its [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) by the [polarization identity](../../../../../polarization-identity.md),

$$
B(x,y)=\frac{Q(x+y)-Q(x)-Q(y)}2,\qquad Q(x)=B(x,x).
$$

We first construct a diagonal [basis](../../../../../basis.md) by induction on the [dimension](../../../../../dimension-vector-space.md). A zero [quadratic form](../../../../../quadratic-form.md) is already diagonal. Otherwise choose $v$ with $Q(v)\ne0$. Every $x$ has the decomposition

$$
x=\frac{B(x,v)}{Q(v)}v+\left(x-\frac{B(x,v)}{Q(v)}v\right),
$$

whose second term lies in $W=\{w:B(w,v)=0\}$. Also $\mathbb Rv\cap W=\{0\}$, so $V=\mathbb Rv\oplus W$ and $\dim W=n-1$. Apply the induction hypothesis to the restricted [quadratic form](../../../../../quadratic-form.md) on $W$. The cross terms with $v$ vanish, giving a diagonal [basis](../../../../../basis.md) on $V$. Rescale each vector with diagonal coefficient $a\ne0$ by $1/\sqrt{|a|}$, and reorder positive, negative and zero coefficients. This yields

$$
\boxed{Q(x)=\sum_{i=1}^p x_i^2-\sum_{i=p+1}^{p+q}x_i^2.}
$$

No nondegeneracy assumption was used.

For uniqueness, let $V_+$ be the positive coordinate subspace and $V_{\leq0}$ the span of all negative and zero coordinate vectors. Their dimensions are $p$ and $n-p$. Any subspace $W$ on which $Q$ has [positive definiteness](../../../../../positive-definiteness.md) intersects $V_{\leq0}$ only in zero. The [dimension formula for a sum of subspaces](../../../../../dimension-formula-for-a-sum-of-subspaces.md) therefore gives $\dim W\leq p$. Conversely $V_+$ itself has dimension $p$ and positive restriction. Thus $p$ is the largest possible dimension of a positive subspace, an intrinsic description independent of the [basis](../../../../../basis.md). Applying the same argument to $-Q$ shows that $q$ is the largest dimension of a negative subspace. This proves [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md), including uniqueness of the zero count $n-p-q$.

The extremal subspaces themselves need not be unique. For $Q(x,y)=x^2-y^2$, the coordinate axes give one positive and one negative line. For any $t\ne0$, put

$$
u=(\cosh t,\sinh t),\qquad v=(\sinh t,\cosh t).
$$

Then $Q(u)=1$, $Q(v)=-1$, $B(u,v)=0$, and the [determinant](../../../../../determinant.md) of the change of [basis](../../../../../basis.md) is one. **The distinct lines $\mathbb Ru$ and $\mathbb Rv$ give another positive/negative decomposition**, with the same intrinsic counts $p=q=1$.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
