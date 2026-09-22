<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the method to the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) $y'=\lambda y$, so $g(y)=\lambda^2y$, and put $z=h\lambda$. A trial numerical mode $y_n=w^n$ satisfies

$$
F_z(w)=(z^2-7z+15)w^2-16zw-(z^2+7z+15)=0.
$$

For every real $z<0$, the leading coefficient is positive, while

$$
F_z(-1)=2z<0,\qquad\lim_{w\to-\infty}F_z(w)=+\infty.
$$

The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) gives a real amplification root $w<-1$. Its modulus exceeds one although the exact scalar solution is decaying. Therefore

$$
\boxed{\text{The method is not A-stable; it is unstable for every negative real }z.}
$$

For a concrete choice, $z=-1$ gives $23w^2+16w-9=0$, whose negative root is $(-8-\sqrt{271})/23<-1$. This proves [negative-real instability of the symmetric two-derivative formula](../../../../../../negative-real-instability-of-the-symmetric-two-derivative-formula.md) directly, without using either an order barrier or the supplied quadratic criterion. The unstable branch is the [parasitic amplification root](../../../../../../parasitic-amplification-root.md) issuing from $w=-1$ at $z=0$; its small-step expansion is $w=-1+z/15+O(z^2)$, so a negative $z$ moves it outside the unit circle immediately.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
