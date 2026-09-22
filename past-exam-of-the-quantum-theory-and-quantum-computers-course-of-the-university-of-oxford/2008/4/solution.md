<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $d=2^N$ and $\lambda=e^{2\pi i/d}$, with nonnegative integer $N$ so the register exists. The [geometric sum](../../../geometric-series.md) satisfies

$$
\sum_{j=0}^{d-1}\lambda^{j(k-l)}=\begin{cases}d,&k=l\pmod d,\\0,&k\ne l\pmod d.\end{cases}
$$

Consequently the [matrix](../../../matrix.md) $F_+$ with entries $d^{-1/2}\lambda^{jk}$ has $F_+^*F_+=I$. This proves [unitarity](../../../unitary-operator.md) and

$$
\boxed{f(j)=d^{-1/2}\sum_{k=0}^{d-1}\lambda^{-jk}\widehat f(k).}
$$

For a binary output string $j=\sum_{r=1}^Nj_r2^{N-r}$, expansion of the printed [tensor product](../../../tensor-product.md) gives coefficient

$$
d^{-1/2}\prod_{r=1}^N\lambda^{2^{N-r}kj_r}=d^{-1/2}\lambda^{kj}.
$$

Thus the printed product is exactly $F_+|k\rangle$. It is a correct [product decomposition of a Fourier phase state](../../../product-decomposition-of-a-fourier-phase-state.md), but the printed recovery identity has inconsistent signs:

$$
\boxed{\sum_k\widehat f(k)F_+|k\rangle=\sum_jf(-j\bmod d)|j\rangle,}
$$

by the [square of the quantum Fourier transform](../../../square-of-the-quantum-fourier-transform.md). To recover $f(j)$ instead, use $F_-=F_+^*$, replacing every product [phase](../../../phase-waves.md) by its complex conjugate. Equivalently one may reverse the sign in the definition of $\widehat f$. The discrepancy is visible for $d\geq4$ by taking $f$ concentrated at $1$: the printed expression returns the [basis](../../../basis.md) vector at $d-1$. The recovery display also uses $k$ as the summation variable on its right while its summand uses $j$; that dummy variable should be $j$.

For factorization first check $\gcd(3,91)=1$. Successive residues are

$$
3^0,3^1,\ldots,3^6\equiv1,3,9,27,81,61,1\pmod{91}.
$$

The first return is $\boxed{r=6}$. Its half power is $3^3=27$, which is neither $1$ nor $-1$ modulo $91$. Therefore

$$
\boxed{\gcd(27-1,91)=13,\qquad\gcd(27+1,91)=7,\qquad91=7\cdot13.}
$$

In [Shor's algorithm](../../../shor-s-algorithm.md) prepare a uniform exponent register of size $Q=2^n$, conveniently $91^2\leq Q<2\cdot91^2$, and reversibly compute $3^x\bmod91$ into a second register. Measuring that second register, or tracing it out, leaves periodic exponent correlations of period $r$. Conditional on one measured residue, the first register is a superposition over an arithmetic progression of exponents separated by $r$. The [quantum Fourier transform](../../../quantum-fourier-transform-split.md) converts this periodic structure into peaks near $k/Q=s/r$. [Continued fractions](../../../continued-fraction.md) recover $s/r$; when $s$ is coprime to $r$, its denominator is $r$. Verify by [modular exponentiation](../../../modular-exponentiation.md) and repeat when the reduced denominator is insufficient. For this example $Q=16384$ is suitable, and useful peaks include those near $Q/6$ and $5Q/6$. Either transform sign gives the same period information, so the source's inverse-sign error does not invalidate the order-finding mechanism.

The Part C inverse-transform display also prints $j$ as its summation index while the summand uses $k$; that sum must be over $k$, as in the corrected inverse above.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2008](../../2008-split.md)
3. [Past exam of the quantum theory and quantum computers course of the University of Oxford](../../split.md)
4. [Quantum theory and quantum computers course of the University of Oxford](../../../quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
