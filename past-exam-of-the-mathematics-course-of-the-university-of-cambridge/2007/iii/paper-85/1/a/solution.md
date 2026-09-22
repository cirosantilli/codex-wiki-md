<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $p=\dot u$ and extend the system by $\dot\lambda=\dot\kappa=0$. At the zero [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) with zero parameters, the $(u,p)$ block is the [nilpotent matrix](../../../../../../nilpotent-matrix.md) $\begin{pmatrix}0&1\\0&0\end{pmatrix}$, while the $v,w$ [eigenvalues](../../../../../../eigenvalue.md) are $-1,-\tau$. Since $\tau>0$, these are stable. The [extended centre manifold](../../../../../../extended-centre-manifold-for-a-parameter.md) is a graph $v=h(u,p,\lambda,\kappa)$, $w=k(u,p,\lambda,\kappa)$ tangent to the four-dimensional centre space containing the two parameter directions. Its invariance equations are

$$
p h_u+(-\lambda u+\kappa p-uh+suk)h_p=-h+u^2,
$$



$$
p k_u+(-\lambda u+\kappa p-uh+suk)k_p=-\tau k+u^2/\tau.
$$

For the quadratic jets in the ordinary total degree, the coefficient multiplying $h_p,k_p$ has no linear part. Hence $p\partial_u h_2=-h_2+u^2$ and $p\partial_u k_2=-\tau k_2+u^2/\tau$. With $h_2=a u^2+bup+cp^2$, comparison gives $a=1$, $b=-2$, $c=2$. The second graph is obtained in the same way. Terms involving parameters at quadratic order have zero forcing and vanish. Thus the [quadratic centre manifold for a pair of linear filters](../../../../../../quadratic-centre-manifold-for-a-pair-of-linear-filters.md) is

$$
\boxed{v=u^2-2up+2p^2+O(3),\qquad
w=\frac{u^2}{\tau^2}-\frac{2up}{\tau^3}+\frac{2p^2}{\tau^4}+O(3).}
$$

Substitution into the centre equations gives the cubic terms

$$
\ddot u+\lambda u=\kappa\dot u+\left(\frac{s}{\tau^2}-1\right)u^3
+2\left(1-\frac{s}{\tau^3}\right)u^2\dot u
+2\left(\frac{s}{\tau^4}-1\right)u\dot u^2+O(4).
$$

The last displayed cubic term is absent from the proposed second-order approximation, so its omission needs the weighted scaling rather than an ordinary-degree truncation.

Under the hinted scaling $u=\varepsilon\tilde u$, $\kappa=\varepsilon\tilde\kappa$, $\lambda=\varepsilon^2\tilde\lambda$, $d/dt=\varepsilon d/d\tilde t$, one has $p=O(\varepsilon^2)$ and $\dot p=O(\varepsilon^3)$. The invariance equations at weighted orders two and three give $v=u^2-2up+O(\varepsilon^4)$ and $w=u^2/\tau^2-2up/\tau^3+O(\varepsilon^4)$. In particular no additional parameter-dependent weighted-order-three graph terms appear. Therefore the $u\dot u^2$ term and the omitted manifold corrections affect the reduced acceleration only at order $\varepsilon^5$, whereas $u^3$ has order $\varepsilon^3$ and $u^2\dot u$ order $\varepsilon^4$. After division by $\varepsilon^3$, the slow equation is

$$
\tilde u''+\tilde\lambda\tilde u
=\tilde\kappa\tilde u'+\left(\frac{s}{\tau^2}-1\right)\tilde u^3
+2\varepsilon\left(1-\frac{s}{\tau^3}\right)\tilde u^2\tilde u'+O(\varepsilon^2).
$$

This proves why the stated approximation retains the leading nonlinear restoring force and its first nonlinear damping correction. The [centre manifold theorem](../../../../../../centre-manifold-theorem.md) removes the exponentially decaying transverse directions, while the retained generic coefficients determine the nearby reduced [bifurcations](../../../../../../bifurcation.md). It is a local asymptotic description, not an exact global reduction. If either relevant coefficient vanishes, higher-order terms may be needed to resolve that degeneracy; the two extreme $s$ cases in part (b), with $\tau=1$, avoid it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
