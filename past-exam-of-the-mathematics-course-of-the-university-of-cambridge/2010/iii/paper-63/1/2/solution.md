<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Yes: this is an A-stable third-order method.** Its second derivative is essential; the [Second Dahlquist barrier](../../../../../../second-dahlquist-barrier.md) applies to ordinary first-derivative [linear multistep methods](../../../../../../linear-multistep-method.md), not this [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md).

Apply the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) $y'=\lambda y$ and put $z=h\lambda$. The amplification [polynomial](../../../../../../polynomial-split.md) is

$$
Q(z)\zeta^2-8\zeta+1=0,\qquad Q(z)=7-6z+2z^2.
$$

We verify the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) throughout $\operatorname{Re}z\le0$. For a quadratic $a\zeta^2+b\zeta+c$ with $|a|>|c|$, the [complex quadratic Schur criterion](../../../../../../complex-quadratic-schur-criterion.md) is

$$
|\overline a b-c\overline b|<|a|^2-|c|^2
$$

for both roots to be strictly inside the [unit disk](../../../../../../unit-disk.md). Here is a brief justification of the criterion rather than just a root plot. Set $P^\#(\zeta)=\zeta^2\overline{P(1/\overline\zeta)}$. The [polynomial](../../../../../../polynomial-split.md) $\overline aP-cP^\#$ is $\zeta(D\zeta+E)$, where $D=|a|^2-|c|^2$ and $E=\overline a b-c\overline b$. Its two roots are inside precisely when $|E|<D$. On the [unit circle](../../../../../../complex-unit-circle.md) $|P^\#|=|P|$, and $|c|<|a|$, so the [Rouche theorem](../../../../../../rouche-s-theorem.md) equates its interior root count with that of $P$. A boundary zero of $P$ would also be a boundary zero of the transformed [polynomial](../../../../../../polynomial-split.md), which the strict inequality excludes. This proves the strict criterion; the non-strict form follows by continuity, with any unit root simple because $|c/a|<1$.

For the present [polynomial](../../../../../../polynomial-split.md) it is enough to show $8|Q-1|<|Q|^2-1$, except at $z=0$. Write $z=-r+iy$, $r\ge0$, and put $k=r^2+3r$, $s=y^2$. Then

$$
Q=(7+2k-2s)-i(6+4r)y,
\qquad X:=|Q|^2-1=(2k+6)(2k+8)+8(k+1)s+4s^2>0.
$$

Direct expansion gives the nonnegative factorization

$$
X^2-64|Q-1|^2
=16\left[k(k+3)^2(k+8)+4k(k^2+8k+11)s
+2(3k^2+11k+6)s^2+4(k+1)s^3+s^4\right].
$$

Every term is nonnegative, and the sum is strictly positive unless $r=y=0$. Also $|Q|^2=X+1>1$, so the criterion applies. For every nonzero $z$ in the closed left half-plane both amplification roots are strictly inside the [unit disk](../../../../../../unit-disk.md). At $z=0$ they are $1$ and $1/7$, and the unit root is simple. Therefore

$$
\boxed{\text{the method is A-stable}.}
$$

This proof establishes stability of both the principal and parasitic modes, including on the imaginary axis.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
