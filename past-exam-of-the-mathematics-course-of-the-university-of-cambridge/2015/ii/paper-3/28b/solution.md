<h1 id="28b/solution">Solution</h1>

↑ **Parent:** [28B](../28b.md)

There are axis equilibria $E_\pm=(\pm\sqrt\mu,0)$ when $\mu\geq0$, and $E_a=(a,a^2-\mu)$ for every $\mu$. At an axis equilibrium $(x_*,0)$ the eigenvalues of the [Jacobian matrix](../../../../../jacobian-matrix.md) are $2x_*$ and $a-x_*$. Thus a negative axis root is a stable node when $a<x_*$ and a saddle when $a>x_*$. A positive axis root is an unstable node when $a>x_*$ and a saddle when $a<x_*$. Equalities give a zero eigenvalue.

At $E_a$,

$$
J=\begin{pmatrix}2a&-1\\\mu-a^2&0\end{pmatrix},\qquad \lambda_\pm=a\pm\sqrt{2a^2-\mu}.
$$

It is a saddle for $\mu<a^2$. For $\mu>a^2$, it is stable if $a<0$, unstable if $a>0$, with real node eigenvalues for $a^2<\mu\leq2a^2$ and a focus for $\mu>2a^2$. At $\mu=2a^2$ the node-focus transition is not a bifurcation of hyperbolicity when $a\ne0$. For $a=0$, $E_a$ has imaginary eigenvalues when $\mu>0$ and the linearized system is a centre. For $a\ne0$, the candidate local bifurcation values are **$\boxed{\mu=0\ \hbox{and}\ \mu=a^2}$**. When $a=0$ these zero-eigenvalue events coincide at $\mu=0$, while the off-axis equilibrium also has zero-real-part imaginary eigenvalues for every $\mu>0$.

The [centre manifold theorem](../../../../../centre-manifold-theorem.md) reduces local dynamics near zero-real-part eigenvalues to an invariant manifold tangent to their eigenspace; transverse directions with nonzero real parts retain their stable or unstable character. For a varying parameter, adjoin $\dot\mu=0$ and use an [extended centre manifold for a parameter](../../../../../extended-centre-manifold-for-a-parameter.md).

Take $a=1$. At $\mu=0$ near the origin, $y=0$ is an exact extended centre manifold. Its reduced equation is

$$
\boxed{\dot x=x^2-\mu,\qquad\dot\mu=0.}
$$

This is a [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md): no nearby axis equilibria for $\mu<0$, one at zero, and two for $\mu>0$. The transverse eigenvalue is positive, so the negative root is a saddle and the positive root an unstable node for small positive $\mu$.

At $\mu=1$, put $u=x-1$, $v=y$, $\nu=\mu-1$. Then $\dot u=2u+u^2-v-\nu$, $\dot v=-uv$, $\dot\nu=0$. Write the extended centre manifold as $u=h(v,\nu)$. Its invariance equation is $h_v(-hv)=2h+h^2-v-\nu$. Matching degrees gives

$$
h(v,\nu)=\frac{v+\nu}{2}-\frac{v^2}{4}-\frac{3v\nu}{8}-\frac{\nu^2}{8}+O((|v|+|\nu|)^3).
$$

Hence **the reduced dynamics are**

$$
\boxed{\dot v=-\frac12v(v+\nu)+O((|v|+|\nu|)^3),\qquad\dot\nu=0.}
$$

The exact equilibrium branches are $v=0$ and $v=-\nu$, crossing at zero and exchanging stability in the centre direction. This is a [transcritical bifurcation](../../../../../transcritical-bifurcation.md); the transverse eigenvalue remains positive. For $\nu<0$ the axis branch is an unstable node and the off-axis branch a saddle; for $\nu>0$ their roles reverse locally.

When $a=0$, the two parameter values merge and the origin at $\mu=0$ has a double zero eigenvalue with nonzero nilpotent linear part. The centre manifold is then two-dimensional, so the preceding one-dimensional classifications cannot simply be reused. Also the off-axis branch has imaginary eigenvalues for every $\mu>0$, with identically zero trace: this is not a generic [Hopf bifurcation](../../../../../hopf-bifurcation.md) obtained by varying $\mu$. These degeneracies already follow without computing a new normal form.

## ↑ Ancestors (10)

1. [28B](../28b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
