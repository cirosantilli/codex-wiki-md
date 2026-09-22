<h1 id="12k/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the intercepted ciphertexts be

$$
c_i\equiv m^{e_i},\qquad c_j\equiv m^{e_j}\pmod N.
$$

Since $\gcd(e_i,e_j)=1$, the extended Euclidean algorithm gives integers $a,b$ with $ae_i+be_j=1$. The [common-modulus RSA attack](../../../../../../../common-modulus-rsa-attack.md) recovers

$$
\boxed{m\equiv c_i^ac_j^b\pmod N}.
$$

Negative powers are evaluated using modular inverses. If an inverse does not exist, its greatest common divisor with $N$ already factors the [modulus](../../../../../../../modulus.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12K](../../../12k.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
