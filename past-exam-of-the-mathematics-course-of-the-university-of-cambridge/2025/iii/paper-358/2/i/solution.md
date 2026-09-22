<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $T=A-zI$. We use the following closed-range lemma:

$$
0\notin\operatorname{Sp}_{\rm ess}(T^*T)
\quad\Longleftrightarrow\quad
T\text{ is upper semi-Fredholm}.
$$

Indeed,

$$
\ker(T^*T)=\ker T.
$$

Away from this kernel, zero is separated from the spectrum of the positive self-adjoint operator $T^*T$ exactly when

$$
\|Tx\|\geq c\|x\|,
\qquad x\perp\ker T,
$$

for some $c>0$. This is equivalent to closed range. Zero is then absent from the essential spectrum exactly when $\dim\ker T<\infty$. Similarly,

$$
0\notin\operatorname{Sp}_{\rm ess}(TT^*)
\quad\Longleftrightarrow\quad
T\text{ is lower semi-Fredholm},
$$

because $\ker T^*=(\operatorname{ran}T)^\perp$ measures the cokernel.

Applying the lecture definitions of the three [essential spectra of a closed operator](../../../../../../essential-spectrum-of-a-closed-operator.md) now gives

$$
\boxed{
\operatorname{Sp}_{\rm ess,1}(A)
=\left\{z:
0\in\operatorname{Sp}_{\rm ess}(T^*T)
\cap\operatorname{Sp}_{\rm ess}(TT^*)\right\}},
$$



$$
\boxed{
\operatorname{Sp}_{\rm ess,2}(A)
=\left\{z:
0\in\operatorname{Sp}_{\rm ess}(T^*T)\right\}},
$$

and

$$
\boxed{
\operatorname{Sp}_{\rm ess,3}(A)
=\left\{z:
0\in\operatorname{Sp}_{\rm ess}(T^*T)
\cup\operatorname{Sp}_{\rm ess}(TT^*)\right\}}.
$$

If $A$ is normal, so is $T$. The spectral theorem gives

$$
T^*T=|T|^2,
$$

and maps the spectral mass of $T$ at $0$ exactly to the spectral mass of $T^*T$ at $0$. Thus zero is isolated with finite multiplicity for $T^*T$ exactly when $z$ is an isolated eigenvalue of finite multiplicity for $A$. Consequently

$$
\boxed{
\operatorname{Sp}_{\rm d}(A)
=\{z:0\in\operatorname{Sp}_{\rm d}(T^*T)\}}.
$$

Normality is essential. Let $Ue_j=e_{j+1}$ be the unilateral shift and take $A=U^*$. Its spectrum is the closed unit disk, so $0$ is not in the [discrete spectrum](../../../../../../discrete-spectrum.md). But

$$
A^*A=UU^*=I-P_{\{e_1\}},
$$

whose zero eigenvalue is isolated and simple. Hence $0\in\operatorname{Sp}_{\rm d}(A^*A)$ while $0\notin\operatorname{Sp}_{\rm d}(A)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
