<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $T=\tanh(ax)$ and $S=\operatorname{sech}^2(ax)$. Using

$$
T'=aS,
\qquad
S'=-2aST,
$$

two differentiations of

$$
\psi(x)=Ne^{ikx}(aT-ik)
$$

give

$$
-\frac{\hbar^2}{2m}\psi''
-\frac{\hbar^2a^2}{m}S\psi
=\frac{\hbar^2k^2}{2m}\psi.
$$

Thus it solves the time-independent [Schrödinger equation](../../../../../../schrodinger-equation.md) in the stated [Pöschl-Teller potential](../../../../../../poschl-teller-potential.md), with

$$
\boxed{E=\frac{\hbar^2k^2}{2m}}.
$$

As $x\to-\infty$ and $x\to+\infty$, respectively,

$$
\psi(x)\sim N(-a-ik)e^{ikx},
\qquad
\psi(x)\sim N(a-ik)e^{ikx}.
$$

There is no left-moving term, so this is a [reflectionless potential](../../../../../../reflectionless-potential.md):

$$
\boxed{P_{\rm ref}=0}.
$$

The incident and transmitted amplitudes have equal modulus because

$$
|-a-ik|^2=|a-ik|^2=a^2+k^2.
$$

Hence

$$
\boxed{P_{\rm tr}=1}.
$$

Now set $k=i\lambda$ with $\lambda>0$. Then

$$
\psi(x)=Ne^{-\lambda x}\bigl(a\tanh(ax)+\lambda\bigr),
\qquad
E=-\frac{\hbar^2\lambda^2}{2m}.
$$

At $+\infty$ this decays for every positive $\lambda$. At $-\infty$, however, the factor tends to $\lambda-a$ while $e^{-\lambda x}$ grows. Normalizability therefore requires $\lambda=a$. In that case

$$
\psi(x)=Na\,e^{-ax}(1+\tanh ax)
=Na\,\operatorname{sech}(ax),
$$

which decays at both ends. The bound-state energy is

$$
\boxed{E=-\frac{\hbar^2a^2}{2m}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
