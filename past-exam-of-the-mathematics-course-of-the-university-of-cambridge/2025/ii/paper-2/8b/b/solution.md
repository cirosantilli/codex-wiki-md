<h1 id="8b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\epsilon=|E|>0$. On the energy surface,

$$
\frac{p^2}{2m}=\frac1{|q|}-\epsilon\geq0,
$$

so

$$
\boxed{|q|\leq q_{\max}=\frac1\epsilon.}
$$

Equality occurs at a turning point, so this is the smallest possible bound.

Using the natural collision continuation through the singular point, a full orbit runs between both turning points. Hence

$$
I=\frac1{2\pi}\oint p\,dq
=\frac2\pi\int_0^{1/\epsilon}
\sqrt{2m\left(\frac1q-\epsilon\right)}\,dq.
$$

Set $q=x^2/\epsilon$. Then

$$
\int_0^{1/\epsilon}\sqrt{2m\left(\frac1q-\epsilon\right)}\,dq
=2\sqrt{\frac{2m}{\epsilon}}
\int_0^1\sqrt{1-x^2}\,dx
=\frac\pi2\sqrt{\frac{2m}{\epsilon}}.
$$

Therefore

$$
\boxed{I=\sqrt{\frac{2m}{|E|}}.}
$$

If instead one identifies the singularity as a reflecting endpoint and regards one half-line as the orbit, the action is half this value; the following scaling is identical.

Adiabatic invariance keeps $m/|E|$ constant. Thus doubling $m$ doubles $|E|$:

$$
\boxed{|E|_{\rm final}=2|E|_{\rm initial},
\qquad E_{\rm final}=2E_{\rm initial}.}
$$

The energy becomes twice as negative.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
