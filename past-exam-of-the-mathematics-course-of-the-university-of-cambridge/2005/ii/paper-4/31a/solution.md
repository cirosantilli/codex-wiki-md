<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

Assume the change of variable is locally invertible with $\xi'>0$; the Liouville-Green choice below requires $q>0$ away from [turning points](../../../../../turning-point.md). Write $r=dx/d\xi$ and $w=\sqrt r\,W$. With dots denoting $\xi$ [derivatives](../../../../../derivative.md),

$$
w_x=r^{-1/2}\dot W+\frac{\dot r}{2r^{3/2}}W,\qquad
w_{xx}=r^{-3/2}\ddot W+
\left(\frac{\ddot r}{2r^{5/2}}-\frac{3\dot r^2}{4r^{7/2}}\right)W.
$$

The first-derivative terms cancel. Substitution into $w_{xx}=qw$ gives

$$
\boxed{\ddot W=
\left[r^2q-\frac{\ddot r}{2r}+\frac{3\dot r^2}{4r^2}\right]W
=\left[r^2q+r^{1/2}\frac{d^2}{d\xi^2}(r^{-1/2})\right]W}.
$$

For $\xi'=\sqrt q$, we have $r=q^{-1/2}$ and $r^2q=1$. Expressing the [derivative](../../../../../derivative.md) correction in $x$ yields

$$
\boxed{\ddot W=(1+\varphi)W,\qquad
\varphi=-q^{-3/4}(q^{-1/4})''
=\frac{q''}{4q^2}-\frac{5(q')^2}{16q^3}}.
$$

If this correction is negligible over the relevant scale, $W$ is approximately $e^{\pm\xi}$, so the [Liouville-Green exponential ansatz](../../../../../liouville-green-exponential-ansatz.md) is

$$
\boxed{w_\pm=q^{-1/4}\exp\!\left(\pm\int\sqrt q\,dx\right)}.
$$

Zeros of $q$ are [turning points](../../../../../turning-point.md) at which this coordinate and approximation need separate treatment.

For the stated Whittaker equation put $\kappa=s(s-1)$. At large positive $x$, $q=1/4+\kappa/x^2>0$, $q^{-1/4}\to\sqrt2$, and

$$
\int\sqrt q\,dx=x/2-\kappa/x+O(x^{-3}).
$$

After normalizing the arbitrary leading constants, this suggests the two exponentials times inverse-power series given in the question.

To derive the coefficients, write $w_A=e^{x/2}F(x)$ with $F=\sum_{n\ge0}a_nx^{-n}$ and $a_0=1$. The equation becomes $F''+F'=\kappa x^{-2}F$. Matching the coefficient of $x^{-n-1}$ gives

$$
-na_n+[n(n-1)-\kappa]a_{n-1}=0,\qquad
a_n=-\frac{(s-n)(s+n-1)}n\,a_{n-1}.
$$

Thus

$$
\boxed{a_n=\frac{(-1)^n}{n!}
(s-n)(s-n+1)\cdots(s+n-1)}.
$$

Similarly $w_B=e^{-x/2}G$ gives $G''-G'=\kappa x^{-2}G$, so $b_n=(-1)^na_n$. These are asymptotic series, not generally convergent series; for integer values making a recurrence factor zero they terminate. The coefficient comparison uses exactly the stated permission to differentiate asymptotically term by term.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
