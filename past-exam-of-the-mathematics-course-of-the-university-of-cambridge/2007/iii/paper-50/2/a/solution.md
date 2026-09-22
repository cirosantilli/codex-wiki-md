<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The normalized [Fock vacuum](../../../../../../fock-vacuum.md) obeys $a_{\mathbf p}|0\rangle=0$ for every momentum and $\langle0|0\rangle=1$. Taking adjoints gives $\langle0|a_{\mathbf p}^\dagger=0$. Of the four products in the mode expansion of $\phi(x)\phi(y)$, only $a_{\mathbf p}a_{\mathbf q}^\dagger$ has a nonzero [vacuum expectation value](../../../../../../vacuum-expectation-value.md). The [commutator](../../../../../../commutator.md) implies

$$
\langle0|a_{\mathbf p}a_{\mathbf q}^\dagger|0\rangle=(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q).
$$

Consequently

$$
\begin{aligned}
\langle0|\phi(x)\phi(y)|0\rangle
&=\int\frac{d^3p\,d^3q}{(2\pi)^6\sqrt{2E_{\mathbf p}\,2E_{\mathbf q}}}(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q)e^{-ipx+iqy}\\
&=\boxed{\int\frac{d^3p}{(2\pi)^3\,2E_{\mathbf p}}e^{-ip\cdot(x-y)}}.
\end{aligned}
$$

This unordered [Wightman function](../../../../../../wightman-function.md) differs from the time-ordered [Feynman propagator](../../../../../../feynman-propagator.md) when the temporal ordering is reversed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
