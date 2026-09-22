<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the physical-space [L2 norm](../../../../../../l2-norm.md) use $\|h\|_2^2=\mathbb E_x|h(x)|^2$. By part (i) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md),

$$
\|f-g\|_2^2=\sum_r|1-\omega^{-ru}|^2|\widehat a(r)|^4.
$$

Split this sum into the [large spectrum](../../../../../../large-spectrum.md) $K$ and its complement. Because $u$ belongs to the [Bohr set](../../../../../../bohr-set.md) in the question, for $r\in K$,

$$
|1-\omega^{-ru}|=|1-\omega^{ru}|\leq\varepsilon.
$$

Consequently the contribution from $K$ is at most $\varepsilon^2\sum_r|\widehat a(r)|^4\leq\varepsilon^2\alpha^3$ by part (ii). Outside $K$, $|\widehat a(r)|<\theta$, and $|1-\omega^{-ru}|\leq2$. Thus that contribution is at most

$$
4\theta^2\sum_{r\notin K}|\widehat a(r)|^2\leq4\theta^2\alpha.
$$

Adding the estimates proves

$$
\boxed{\|f-g\|_2^2\leq\varepsilon^2\alpha^3+4\theta^2\alpha.}
$$

The argument also covers empty $A$ or empty $K$. As usual the radius and threshold are nonnegative; a negative radius makes the premise empty whenever $K$ is nonempty. The estimate expresses [Bohr-set almost periodicity of a convolution](../../../../../../bohr-set-almost-periodicity-of-a-convolution.md): a [translation of a function](../../../../../../translation-of-a-function.md) by an element of the [Bohr set](../../../../../../bohr-set.md) barely changes the large [Fourier coefficients on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md), while the small ones have little total energy.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
