<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [characteristic polynomial](../../../../../../characteristic-polynomial.md) in the convention $p(\lambda)=\det(\lambda I-A)$:

$$
p(\lambda)=(\lambda+1)(\lambda-\alpha)(\lambda-1)-\epsilon(3\lambda-1).
$$

For fixed $\alpha>0$ with $\alpha\ne1$, all three limiting [eigenvalues](../../../../../../eigenvalue.md) are simple. Expanding this [polynomial](../../../../../../polynomial-split.md) at each root, or applying [first-order perturbation of a simple eigenvalue](../../../../../../first-order-perturbation-of-a-simple-eigenvalue.md), gives

$$
\boxed{\begin{aligned}
\lambda_{-1}&=-1-\frac{2\epsilon}{\alpha+1}+O(\epsilon^2),\\
\lambda_\alpha&=\alpha+\frac{(3\alpha-1)\epsilon}{(\alpha+1)(\alpha-1)}+O(\epsilon^2),\\
\lambda_1&=1-\frac{\epsilon}{\alpha-1}+O(\epsilon^2).
\end{aligned}}
$$

These are fixed-$\alpha$ [asymptotic expansions](../../../../../../asymptotic-expansion.md), not uniform through $\alpha=1$. At $\alpha=1/3$ the displayed correction to $\lambda_\alpha$ vanishes because $\lambda=1/3$ is an exact root for every $\epsilon$; there is no second nonzero term for that branch.

The two roots near $1$ interact when the correction $\epsilon/(\alpha-1)$ is comparable to their unperturbed gap $\alpha-1$. Thus the [distinguished limit](../../../../../../distinguished-limit.md) is $\alpha=1+d\sqrt\epsilon$, with bounded real $d$. Set $h=\sqrt\epsilon$ and $\lambda=1+hL+h^2N+\cdots$. The [polynomial](../../../../../../polynomial-split.md) becomes

$$
(2+\delta)\delta(\delta-dh)-h^2(2+3\delta)=0,\qquad \delta=\lambda-1.
$$

At orders $h^2$ and $h^3$,

$$
L(L-d)=1,\qquad N(2L-d)=L.
$$

With $D=\sqrt{d^2+4}$, the two interacting [eigenvalues](../../../../../../eigenvalue.md) are

$$
\boxed{\lambda_\pm=1+\frac{h}{2}(d\pm D)+\frac{h^2}{2}\left(1\pm\frac dD\right)+O(h^3),\qquad \lambda_{-1}=-1-\epsilon+O(\epsilon^{3/2}).}
$$

The $h^2$ correction to the pair is included to resolve the next perturbative term as well as the leading splitting. In particular the previously excluded fixed case $\alpha=1$ is $d=0$:

$$
\boxed{\lambda_\pm=1\pm\sqrt\epsilon+\frac\epsilon2+O(\epsilon^{3/2}),\qquad \lambda_{-1}=-1-\epsilon+O(\epsilon^2).}
$$

The half-integer powers reflect [square-root splitting of a defective double eigenvalue](../../../../../../square-root-splitting-of-a-defective-double-eigenvalue.md): the limiting [matrix](../../../../../../matrix.md) has a nontrivial [Jordan block](../../../../../../jordan-block.md) at $1$.

For matching, write $\Delta=\alpha-1$ and take the overlap $\sqrt\epsilon\ll|\Delta|\ll1$. For $d\to+\infty$, $L_+=d+d^{-1}+O(d^{-3})$, $N_+=1+O(d^{-2})$, while $L_-=-d^{-1}+O(d^{-3})$, $N_-=O(d^{-2})$. Consequently the distinguished branches reduce to

$$
\lambda_{\alpha}=\alpha+\frac\epsilon\Delta+\epsilon+O(\epsilon\Delta)+O(\epsilon^2/|\Delta|^3),\qquad
\lambda_1=1-\frac\epsilon\Delta+O(\epsilon^2/|\Delta|^3).
$$

The regular coefficient satisfies $(3\alpha-1)/[(\alpha+1)(\alpha-1)]=1/\Delta+2/(2+\Delta)=1/\Delta+1+O(\Delta)$, proving agreement. For $d\to-\infty$ the labels $+$ and $-$ exchange roles and the same matching holds. The isolated negative branch also matches because $-2/(\alpha+1)=-1+O(\Delta)$. As a spectral check, [positive diagonal symmetrization of a matrix](../../../../../../positive-diagonal-symmetrization-of-a-matrix.md) transforms this tridiagonal [matrix](../../../../../../matrix.md) to a real [symmetric matrix](../../../../../../symmetric-matrix.md) with off-diagonal entries $\sqrt{2\epsilon}$ and $\sqrt\epsilon$; its [eigenvalues](../../../../../../eigenvalue.md) are real for positive $\epsilon$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
