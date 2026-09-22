<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Since $u$ and $v$ are [harmonic conjugates](../../../../../harmonic-conjugate.md), $f=u+iv$ is a [holomorphic function](../../../../../holomorphic-function.md) on $D$, with $u_x=v_y$ and $u_y=-v_x$. The entire function $w\mapsto e^{iw^2}$ can be composed with $f$. Its value is

$$
e^{if^2}=e^{i(u^2-v^2+2iuv)}=e^{-2uv}\bigl[\cos(u^2-v^2)+i\sin(u^2-v^2)\bigr]=U+iV.
$$

By the complex [chain rule](../../../../../chain-rule.md) the composition is holomorphic on $D$, so its real and imaginary parts obey the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). They are harmonic as well: differentiating those equations gives $U_{xx}+U_{yy}=V_{yx}-V_{xy}=0$ and likewise $V_{xx}+V_{yy}=0$. Hence **$U,V$ are a pair of harmonic conjugates on $D$**. No simple-connectivity assumption is needed because the conjugate pair is already supplied globally. The PDF has $e^{-2uv}$ in both expressions; the differing TeX exponents are transcription defects.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
