<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

Compatibility of the auxiliary system, computed on a fundamental [matrix](../../../../../matrix.md) of solutions, gives the [zero-curvature condition](../../../../../zero-curvature-condition.md)

$$
\boxed{U_t-V_x+[U,V]=0.}
$$

Indeed equality of the mixed [derivatives](../../../../../derivative.md) gives $(U_t+UV-V_x-VU)\Psi=0$. A single possibly zero vector solution would not justify the [matrix](../../../../../matrix.md) identity; compatibility means a full fundamental family.

Put $H=W_t-VW$. Using the [zero-curvature condition](../../../../../zero-curvature-condition.md) gives $H_x=UH$. At $x=0$, $W_t=0$ and hence $H(0)=-V(0)$. Uniqueness of the initial-value problem gives $H=-WV(0)$, or $W_t=VW-WV(0)$. Periodicity implies $V(2\pi)=V(0)=v$, so the [monodromy matrix](../../../../../monodromy-matrix.md) $w=W(2\pi)$ obeys the [Lax equation](../../../../../isospectral-lax-equation.md)

$$
\boxed{w_t=[v,w].}
$$

Cyclicity of the trace yields $\frac d{dt}\operatorname{tr}(w^k)=k\operatorname{tr}(w^{k-1}[v,w])=0$ for every $k\geq1$.

There is a genuine factor-of-two error in the printed sine-Gordon pair. Assign the second printed [matrix](../../../../../matrix.md) to $U$ and the first to $V_{\rm print}$:

$$
U=\frac i2\begin{pmatrix}2\lambda&u_x\\u_x&-2\lambda\end{pmatrix},\qquad
V_{\rm print}=\frac1{2i\lambda}\begin{pmatrix}\cos u&-i\sin u\\i\sin u&-\cos u\end{pmatrix}.
$$

Direct multiplication gives

$$
U_t-(V_{\rm print})_x+[U,V_{\rm print}]
=\frac i2\begin{pmatrix}0&u_{xt}-2\sin u\\u_{xt}-2\sin u&0\end{pmatrix}.
$$

Thus **the printed [matrices](../../../../../matrix.md) encode $u_{xt}=2\sin u$**.

For the stated [Sine-Gordon equation](../../../../../sine-gordon-equation.md), explicitly repair the first prefactor by taking $V=V_{\rm print}/2$, that is $1/(4i\lambda)$. Its [zero-curvature condition](../../../../../zero-curvature-condition.md) becomes $u_{xt}=\sin u$. For this corrected pair, $\operatorname{tr}(w(t,\lambda)^k)$ is conserved for every $\lambda\ne0$. Since $U$ is entire in $\lambda$, so are $W$ and these traces. Their Taylor coefficients in $\lambda$ supply an infinite family of [first integrals](../../../../../first-integral.md), by the identity theorem extending conservation through $\lambda=0$. At a fixed spectral parameter the higher traces of a $2\times2$ [matrix](../../../../../matrix.md) are related by the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md); **no independence of the resulting [first integrals](../../../../../first-integral.md) is claimed**.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
