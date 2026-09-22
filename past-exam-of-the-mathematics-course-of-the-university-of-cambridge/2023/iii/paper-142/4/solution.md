<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The cofibration

$$
S(E)\longrightarrow D(E)\longrightarrow\operatorname{Th}(E)
$$

gives the long exact sequence of a pair in [Topological K-theory](../../../../../topological-k-theory.md). Identify $D(E)$ with $X$ by deformation retraction and use multiplication by the [K-theory Thom class](../../../../../k-theory-thom-class.md)

$$
\lambda_E\in\widetilde K^0(\operatorname{Th}(E))
$$

to identify the relative term with $K^*(X)$. Pullback along the zero section sends $\lambda_E$ to the [K-theory Euler class](../../../../../k-theory-euler-class.md)

$$
e^K(E)=\Lambda_{-1}(\overline E).
$$

The map from the relative term to $K^*(D(E))$ is therefore multiplication by $e^K(E)$, giving the [K-theory Gysin sequence of a sphere bundle](../../../../../k-theory-gysin-sequence-of-a-sphere-bundle.md)

$$
\cdots\to
K^i(X)\xrightarrow{\cdot e^K(E)}K^i(X)
\xrightarrow{p^*}K^i(S(E))
\xrightarrow{p_!}K^{i+1}(X)
\to\cdots.
$$

For

$$
Y=S(\gamma_{\mathbb C}^{1,n+1}\oplus\gamma_{\mathbb C}^{1,n+1})
$$

over $\mathbb{CP}^n$, put $t=1-[\overline\gamma]$. The [Complex K-theory of complex projective space](../../../../../complex-k-theory-of-complex-projective-space.md) is

$$
K^0(\mathbb{CP}^n)=\mathbb Z[t]/(t^{n+1}),
\qquad
K^{-1}(\mathbb{CP}^n)=0,
$$

and

$$
e^K(\gamma\oplus\gamma)
=(1-[\overline\gamma])^2=t^2.
$$

The Gysin sequence consequently identifies

$$
K^{-1}(Y)
\cong\ker\left(t^2:\mathbb Z[t]/(t^{n+1})\to
\mathbb Z[t]/(t^{n+1})\right)
=\mathbb Z\{t^{n-1},t^n\}
\cong\mathbb Z^2
$$

for $n\geq1$. This is the [Odd K-theory of the sphere bundle of two tautological lines](../../../../../odd-k-theory-of-the-sphere-bundle-of-two-tautological-lines.md).

If $n=0$, then the base is a point and $Y=S^3$, so $K^{-1}(Y)\cong\mathbb Z$ by [Bott periodicity](../../../../../bott-isomorphism.md).

The [cannibalistic class](../../../../../cannibalistic-class.md) is defined by the identity

$$
\psi^k(\lambda_E)=\rho^k(E)\lambda_E
$$

for the [Adams operation](../../../../../adams-operation.md) $\psi^k$. The Thom class of a direct sum is the product of the pulled-back Thom classes. Applying the ring homomorphism $\psi^k$ gives

$$
\rho^k(E\oplus E')=\rho^k(E)\rho^k(E').
$$

If $L$ is a line bundle, restriction along the zero section gives

$$
(1-\overline L^k)
=\rho^k(L)(1-\overline L),
$$

so

$$
\rho^k(L)
=1+\overline L+\cdots+\overline L^{k-1}.
$$

Let $\delta:K^{-1}(S(E))\to\widetilde K^0(\operatorname{Th}(E))$ be the boundary map. By definition of $p_!$,

$$
\delta x=\lambda_Ep_!(x).
$$

The natural operation $\psi^k$ commutes with $\delta$, and therefore

$$
\lambda_Ep_!(\psi^kx)
=\psi^k(\lambda_Ep_!(x))
=\rho^k(E)\lambda_E\psi^k(p_!(x)).
$$

Cancelling the Thom class proves the [Adams operation and the boundary pushforward of a sphere bundle](../../../../../adams-operation-and-the-boundary-pushforward-of-a-sphere-bundle.md) formula

$$
p_!(\psi^kx)=\rho^k(E)\psi^k(p_!(x)).
$$

Choose the basis $a,b$ of $K^{-1}(Y)$ characterized by

$$
p_!(a)=t^{n-1},
\qquad
p_!(b)=t^n.
$$

For $E=\gamma\oplus\gamma$,

$$
\rho^2(E)=(1+\overline\gamma)^2=(2-t)^2,
\qquad
\psi^2(t)=1-\overline\gamma^2=2t-t^2=t(2-t).
$$

Modulo $t^{n+1}$, this gives

$$
\begin{aligned}
p_!(\psi^2a)
&=(2-t)^2\bigl(t(2-t)\bigr)^{n-1}\\
&=2^{n+1}t^{n-1}-(n+1)2^nt^n,\\
p_!(\psi^2b)
&=(2-t)^2\bigl(t(2-t)\bigr)^n
=2^{n+2}t^n.
\end{aligned}
$$

Since $p_!$ identifies $K^{-1}(Y)$ with this kernel, the [Second Adams operation on the odd K-theory of the sphere bundle of two tautological lines](../../../../../second-adams-operation-on-the-odd-k-theory-of-the-sphere-bundle-of-two-tautological-lines.md) is

$$
\psi^2(a)=2^{n+1}a-(n+1)2^nb,
\qquad
\psi^2(b)=2^{n+2}b.
$$

For $n=0$, the single generator of $K^{-1}(S^3)$ is multiplied by $4$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
