<h1 id="18d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $B=b+ic$ with $b>0$. Normalization of the [Gaussian wave packet](../../../../../../gaussian-wave-packet.md) gives $|A|^2\int e^{-2bx^2}\,dx=1$, hence $|A|^2=\sqrt{2b/\pi}$. The supplied [Gaussian integral](../../../../../../gaussian-integral.md) ratio then gives

$$
\boxed{\langle x^2\rangle=\frac1{4b}}.
$$

The [momentum operator](../../../../../../momentum-operator.md) obeys $p\Psi=2i\hbar Bx\Psi$, and direct second differentiation gives $p^2\Psi=(2\hbar^2B-4\hbar^2B^2x^2)\Psi$. Taking the [expectation value](../../../../../../expectation-value.md) and substituting the first result gives

$$
\langle p^2\rangle=2\hbar^2B-\frac{\hbar^2B^2}{b}=\frac{\hbar^2B(2b-B)}b=\frac{\hbar^2|B|^2}b=\boxed{4\hbar^2|B|^2\langle x^2\rangle},
$$

since $2b-B=\bar B$. These are the [second moments of a complex Gaussian wave packet](../../../../../../second-moments-of-a-complex-gaussian-wave-packet.md).

For the solution in part (b), the trigonometric identity

$$
\tan(\phi-it)=\frac{\sin(2\phi)-i\sinh(2t)}{\cos(2\phi)+\cosh(2t)}
$$

gives, writing $D=\cosh(2t)+\cos(2\phi)$,

$$
b=\frac{\sin(2\phi)}{2\hbar D},\qquad |B|^2=\frac{\cosh(2t)-\cos(2\phi)}{4\hbar^2D}.
$$

Thus normalizability requires $\sin(2\phi)>0$, and the exact [expectation values](../../../../../../expectation-value.md) are

$$
\langle x^2\rangle=\frac{\hbar[\cosh(2t)+\cos(2\phi)]}{2\sin(2\phi)},\qquad \langle p^2\rangle=\frac{\hbar[\cosh(2t)-\cos(2\phi)]}{2\sin(2\phi)}.
$$

Since $\cosh(2t)\sim e^{2t}/2$,

$$
\boxed{\langle x^2\rangle\sim\langle p^2\rangle\sim\frac{\hbar}{4\sin(2\phi)}e^{2t}}.
$$

Their difference is the constant $-\hbar\cot(2\phi)$, so the mean [energy](../../../../../../energy.md) $\langle H\rangle=-\hbar\cot(2\phi)/2$ stays constant despite exponential spreading in both observables.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18D](../../18d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
