<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Split the field into disjoint ranges of [Fourier modes](../../../../../../../fourier-mode.md),

$$
\phi_{\rm tot}=\phi+\phi^+,
\qquad
\widetilde\phi(p)=0\ (p^2>\Lambda^2),
\qquad
\widetilde{\phi^+}(p)=0\ \text{unless }\Lambda^2<p^2\leq\Lambda_0^2.
$$

The [Wilsonian effective action](../../../../../../../wilsonian-effective-action.md) is defined by

$$
e^{-S_\Lambda^{\rm eff}[\phi]}
=\int_\Lambda^{\Lambda_0}\mathcal D\phi^+\,
e^{-S_{\Lambda_0}[\phi+\phi^+]}.
$$

Writing $\Delta S[\phi,\phi^+]=S_{\Lambda_0}[\phi+\phi^+]-S_{\Lambda_0}[\phi]$ immediately gives

$$
\boxed{S_\Lambda^{\rm eff}[\phi]=S_{\Lambda_0}[\phi]
-\log\int_\Lambda^{\Lambda_0}\mathcal D\phi^+e^{-\Delta S[\phi,\phi^+]}.}
$$

Quadratic cross terms vanish because the momentum supports do not overlap. For $h_0\ne0$,

$$
\begin{aligned}
\Delta S={}&S_{0,>}[\phi^+]
+\int d^4x\left\{
\frac{h_0}{3!}\left[3\phi^2\phi^++3\phi(\phi^+)^2+(\phi^+)^3\right]\right.\\
&\left.\hspace{31mm}
+\frac{g_0}{4!}\left[4\phi^3\phi^++6\phi^2(\phi^+)^2
+4\phi(\phi^+)^3+(\phi^+)^4\right]\right\},
\end{aligned}
$$

where

$$
S_{0,>}[\phi^+]=\frac12\int d^4x\,
\left[(\partial\phi^+)^2+m_0^2(\phi^+)^2\right].
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 304](../../../../paper-304-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
