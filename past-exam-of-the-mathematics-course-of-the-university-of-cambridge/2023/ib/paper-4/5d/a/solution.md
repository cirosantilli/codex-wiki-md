<h1 id="5d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\theta$ be the angle between $r$ and the positive $z$-axis. By superposition of the [electric potential](../../../../../../electric-potential.md) of point charges,

$$
\Phi(r)=\frac{Q}{4\pi\epsilon_0}
\left(\frac N r-\frac1{|r-d\widehat z|}
-\frac M{|r+d\widehat z|}\right).
$$

For $r>d$, the [Legendre polynomial](../../../../../../legendre-polynomial.md) expansion gives

$$
\frac1{|r\mp d\widehat z|}
=\frac1r\left[1\pm\frac d r\cos\theta
+\frac{d^2}{2r^2}(3\cos^2\theta-1)+O(r^{-3})\right].
$$

Therefore

$$
\boxed{\Phi(r,\theta)=\frac{Q}{4\pi\epsilon_0}\left[
\frac{N-M-1}{r}
+\frac{(M-1)d\cos\theta}{r^2}
-\frac{(M+1)d^2(3\cos^2\theta-1)}{2r^3}
+O(r^{-4})\right]}.
$$

The three displayed terms are respectively the monopole, dipole, and quadrupole terms of the [electric multipole expansion](../../../../../../electric-multipole-expansion.md). In particular, the total charge is $Q(N-M-1)$ and the [electric dipole moment](../../../../../../electric-dipole-moment.md) is $Qd(M-1)\widehat z$. This is the [multipole expansion of three collinear charges](../../../../../../multipole-expansion-of-three-collinear-charges.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
