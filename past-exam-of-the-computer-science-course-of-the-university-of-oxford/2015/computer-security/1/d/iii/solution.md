<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The fact that a nontrivial factor usually appears before a full return does not say that either event appears soon. Each iteration of the [RSA cycling attack](../../../../../../rsa-cycling-attack.md) is inexpensive, but the number of iterations can be enormous. The [multiplicative orders](../../../../../../multiplicative-order.md) governing returns modulo $p$ and $q$ need not be small, and writing down a large return exponent does not provide a fast way to search the preceding iterations.

If this procedure factored arbitrary well-generated [RSA cryptosystem](../../../../../../rsa-cryptosystem.md) moduli in feasible time with substantial success, it would solve the associated [integer factorization](../../../../../../integer-factorization.md) problem efficiently. If it instead rapidly returned the predecessor of a [ciphertext](../../../../../../ciphertext.md) without factoring, it would solve the [RSA inversion problem](../../../../../../rsa-inversion-problem.md). Both are intended to be infeasible for appropriate parameters. Efficient [integer factorization](../../../../../../integer-factorization.md) certainly breaks [RSA cryptosystem](../../../../../../rsa-cryptosystem.md) security; the reverse implication for general [RSA inversion problem](../../../../../../rsa-inversion-problem.md) algorithms is not known.

$$
\boxed{\text{A likely factor before a return does not establish a feasible running time.}}
$$

Thus the stated observation alone provides no serious general attack on well-generated parameters. It also does not prove a lower bound: special moduli or messages with short cycles can be weak, and the hardness claims are computational assumptions.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
