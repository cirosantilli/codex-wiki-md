<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Berezin integral](../../../../../../berezin-integral.md) over independent [Grassmann variables](../../../../../../grassmann-variable.md) selects the coefficient containing every variable. Fix the real orientation by $\int d\omega_1\cdots d\omega_{2m}\,\omega_{2m}\cdots\omega_1=1$. For an [antisymmetric matrix](../../../../../../skew-symmetric-matrix.md) $A$, only the order-$m$ term in the exponential survives:

$$
\frac{(-1)^m}{2^m m!}\left(\sum_{i,j}\omega_iA_{ij}\omega_j\right)^m.
$$

Anticommutation collects its top coefficient into the signed sum over pairings that defines the [Pfaffian](../../../../../../pfaffian.md). Reversing the order of $2m$ variables gives $(-1)^{m(2m-1)}=(-1)^m$, cancelling the prefactor sign. The [real Grassmann Gaussian integral](../../../../../../real-grassmann-gaussian-integral.md) is therefore

$$
\boxed{\int d\omega_1\cdots d\omega_{2m}\,e^{-\omega^TA\omega/2}=\operatorname{Pf}(A)}
$$

with this orientation, and a fixed sign times this answer with other orientations. In dimension two, write $A_{12}=a$; the exponential is $1-a\omega_1\omega_2=1+a\omega_2\omega_1$, and integration gives $a$. Although $\operatorname{Pf}(A)^2=\det A$, writing a positive square root $\sqrt{\det A}$ would give $|a|$ in this test and would lose the correct sign.

For the complex [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md), treat $\theta_a$ and $\bar\theta_a$ as independent integration variables. Every surviving top term contains each $\theta$ and each $\bar\theta$ once. Expanding the exponential assigns one matrix entry from every row and column, and anticommutation supplies the permutation sign. Hence

$$
\boxed{\int\prod_{a=1}^n d\theta_a\prod_{a=1}^n d\bar\theta_a\,e^{-\bar\theta^TM\theta}=C_n\det M,}
$$

where $C_n$ is a nonzero constant fixed by the order and normalization of the differentials, independent of $M$. This argument works for singular matrices as well and does not assume that $M$ is Hermitian.

For the explicit $n=2$ check, put $Q=\bar\theta_aM_{ab}\theta_b$. Moving all the $\theta$ variables before the barred ones gives

$$
\frac12Q^2=(-M_{11}M_{22}+M_{12}M_{21})\theta_1\theta_2\bar\theta_1\bar\theta_2.
$$

The linear and constant terms integrate to zero. Thus the integral is a fixed orientation sign times $M_{11}M_{22}-M_{12}M_{21}$, exactly the [determinant](../../../../../../determinant.md). Choosing the top-monomial integral to be $-1$ gives $C_2=1$.

For the required [real-complex compatibility of Grassmann Gaussian integrals](../../../../../../real-complex-compatibility-of-grassmann-gaussian-integrals.md), let $u_a=\omega_a$ and $v_a=\omega_{n+a}$. Substitution gives

$$
\bar\theta^TM\theta=\frac12\left(u^TMu+v^TMv+i u^TMv-i v^TMu\right)=\frac12(u^TMu+v^TMv).
$$

Indeed $v^TMu=-u^TM^Tv=u^TMv$ because the variables anticommute and $M^T=-M$. The real quadratic matrix is consequently $A=\operatorname{diag}(M,M)$, of size $2n$. The linear change of [Grassmann variables](../../../../../../grassmann-variable.md) has a constant nonzero [Berezin integration](../../../../../../berezin-integral.md) Jacobian, so it changes only the allowed normalization factor. For even $n$, the two blocks give

$$
\boxed{\operatorname{Pf}(A)=\operatorname{Pf}(M)^2=\det M.}
$$

For odd $n$, $\det M=\det(-M)=(-1)^n\det M$ implies $\det M=0$. Each of the separate $u$ and $v$ quadratic exponentials has only even degree and cannot saturate an odd number of variables, so the real integral vanishes too. This covers the odd case without attempting to define a [Pfaffian](../../../../../../pfaffian.md) of an odd-dimensional matrix.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
