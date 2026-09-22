<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the outer expansions

$$
y=y_0+\epsilon y_1+\cdots,
\qquad
\omega^2=\omega_0^2+\epsilon\omega_1^2+\cdots.
$$

The reduced leading equation is

$$
y_0''+\omega_0^2y_0=0.
$$

For the symmetric fundamental mode, $y_0=a\cos(\omega_0x)$. The reduced second-order problem can impose the displacement conditions $y_0(\mathord\pm1)=0$ but not both clamped-slope conditions. The smallest positive root is

$$
\boxed{
\omega_0=\frac\pi2,
\qquad
y_0=a\cos\frac{\pi x}{2}}.
$$

Near the right endpoint introduce the stretched coordinate

$$
X_+=\frac{1-x}{\epsilon},
$$

and near the left endpoint use $X_-=(1+x)/\epsilon$. The leading outer solution is $O(\epsilon)$ in either inner region, so put $y=\epsilon Y_0+\cdots$. The dominant inner equation is

$$
Y_0''''-Y_0''=0.
$$

At either endpoint, clamping gives $Y_0(0)=Y_0'(0)=0$, bounded matching excludes the growing exponential, and the outer behavior requires

$$
Y_0\sim\frac{a\pi}{2}X_\pm
\qquad(X_\pm\to\infty).
$$

Thus the two leading inner solutions have the same form:

$$
\boxed{
y_{\rm in}^{\pm}
=\epsilon\frac{a\pi}{2}
\left(X_\pm-1+e^{-X_\pm}\right)}.
$$

They show explicitly that each clamped endpoint has a [boundary layer](../../../../../../boundary-layer.md) of width $O(\epsilon)$.

At order $\epsilon$, the outer equation is

$$
y_1''+\frac{\pi^2}{4}y_1
=-\omega_1^2a\cos\frac{\pi x}{2}.
$$

The symmetric solution is

$$
\boxed{
y_1=b\cos\frac{\pi x}{2}
-\frac{\omega_1^2a}{\pi}
x\sin\frac{\pi x}{2}},
$$

which is the stated resonant particular solution plus a homogeneous normalization term.

As $x=1-\epsilon X_+$ approaches the right endpoint from the outer region,

$$
y_0+\epsilon y_1
\sim\epsilon
\left[
\frac{a\pi}{2}X_+
-\frac{\omega_1^2a}{\pi}
\right].
$$

The large-$X_+$ inner expansion is

$$
y_{\rm in}^+
\sim\epsilon
\left[
\frac{a\pi}{2}X_+
-\frac{a\pi}{2}
\right].
$$

Matching the constant terms gives

$$
\omega_1^2=\frac{\pi^2}{2}.
$$

The left endpoint gives the same condition by symmetry. Therefore

$$
\boxed{
\omega^2
\sim\frac{\pi^2}{4}
+\frac{\pi^2}{2}\epsilon
+O(\epsilon^2)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
