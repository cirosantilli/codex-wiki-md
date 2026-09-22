<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the curvature $-1$ [hyperbolic metric](../../../../../../hyperbolic-metric.md) $ds=2|dz|/(1-|z|^2)$. For the disk [Möbius transformation](../../../../../../mobius-transformation.md) $\phi_w(z)=(z-w)/(1-\overline wz)$, set $r_w(z)=|\phi_w(z)|$. The [hyperbolic distance](../../../../../../hyperbolic-distance.md) satisfies

$$
\rho(w,z)=\log\frac{1+r_w(z)}{1-r_w(z)},\qquad e^{-\rho(w,z)}=\frac{1-r_w(z)}{1+r_w(z)}.
$$

The [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
e^{-\rho(v,w)}e^{-\rho(w,z)}\leq e^{-\rho(v,z)}\leq e^{\rho(v,w)}e^{-\rho(w,z)}.
$$

Thus convergence of the exponential sum is independent of the base point. Taking the base point zero, it is equivalent to the [Blaschke condition](../../../../../../blaschke-condition.md) $\sum_n(1-|z_n|)<\infty$. This condition implies that only finitely many terms lie in any compact subdisk, including finitely many repetitions of any point.

To construct the required [holomorphic function](../../../../../../holomorphic-function.md), for $a\ne0$ define the [Blaschke factor](../../../../../../blaschke-factor.md)

$$
b_a(z)=\frac{|a|}{a}\frac{a-z}{1-\overline az},\qquad b_0(z)=z.
$$

For $|z|\leq R<1$, writing $a=|a|e^{i\alpha}$ gives

$$
1-b_a(z)=(1-|a|)\frac{1+e^{-i\alpha}z}{1-\overline az},\qquad |1-b_a(z)|\leq(1-|a|)\frac{1+R}{1-R}.
$$

Consequently, after the finitely many factors corresponding to small $|a|$ are removed, the sum of $|1-b_a|$ converges uniformly on each compact subdisk. Those factors are uniformly close to one, so their logarithms form an absolutely convergent series there. Their product tail is holomorphic and nonvanishing. Including the finitely many removed factors gives the [Blaschke product](../../../../../../blaschke-product.md)

$$
B(z)=\prod_n b_{z_n}(z)
$$

with exactly the requested zero multiplicities. Each finite product has modulus at most one in the disk, so the limit does too. Hence **$f=B/2$ maps into the open disk and has exactly the prescribed zeros**, proving the implication from the summability condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
