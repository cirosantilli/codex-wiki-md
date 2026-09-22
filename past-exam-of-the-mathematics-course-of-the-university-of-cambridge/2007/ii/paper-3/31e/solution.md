<h1 id="31e/solution">Solution</h1>

↑ **Parent:** [31E](../31e.md)

Use the Fourier convention $\widehat q_0(k)=\int_{\mathbb R}e^{-ikx}q_0(x)dx$ and sufficiently rapidly decaying smooth initial data. A scalar [Lax pair](../../../../../lax-pair.md) for the linear equation is

$$
m_x-ikm=q,\qquad m_t+ik^2m=-kq+iq_x.
$$

Differentiate the first equation in time and use the second and its spatial derivative. The terms involving $m$ and $k$ cancel, leaving $q_t=iq_{xx}$, exactly the linear equation.

The spatially normalized solutions are $m^+=\int_{-\infty}^x e^{ik(x-y)}q(y,t)dy$ for $\operatorname{Im}k>0$, and $m^-=-\int_x^\infty e^{ik(x-y)}q(y,t)dy$ for $\operatorname{Im}k<0$. Integration by parts gives $m^\pm=O(k^{-1})$. Their difference is $e^{ikx}\widehat q(k,t)$; Fourier transformation of the evolution gives $\widehat q(k,t)=e^{-ik^2t}\widehat q_0(k)$. Set $M^\pm=\begin{pmatrix}1&m^\pm\\0&1\end{pmatrix}$. Then

$$
\boxed{M^+=M^-\begin{pmatrix}1&e^{ikx-ik^2t}\widehat q_0(k)\\0&1\end{pmatrix},
\qquad M=I+O(k^{-1}).}
$$

The Cauchy integral solution is $m(k)=(2\pi i)^{-1}\int e^{isx-is^2t}\widehat q_0(s)/(s-k)\,ds$, and reconstruction $q=-i\lim_{k\to\infty}km(k)$ gives the usual inverse Fourier solution.

For the nonlinear deformation, put $D=\operatorname{diag}(1,-1)$ and $Q=\begin{pmatrix}0&q\\\vartheta&0\end{pmatrix}$. The [matrix](../../../../../matrix.md) [Lax pair](../../../../../lax-pair.md) is

$$
\Psi_x=U\Psi,\quad\Psi_t=V\Psi,\qquad
U=\frac{ik}2D+Q,\quad
V=-\frac{ik^2}2D-kQ+iD(Q_x-Q^2).
$$

A direct multiplication gives the off-diagonal entries of $U_t-V_x+[U,V]$ as $q_t-iq_{xx}+2iq^2\vartheta$ and $\vartheta_t+i\vartheta_{xx}-2i\vartheta^2q$, with zero diagonal. Hence compatibility is precisely the two requested nonlinear equations.

Here is a normalized [Riemann-Hilbert problem](../../../../../riemann-hilbert-problem.md) for this pair, in the case without discrete scattering poles. Let $a(k),b(k)$ be its two reflection data determined from the initial spatial scattering problem, and set $\theta=kx-k^2t$. Deform the triangular jump to

$$
\boxed{M^+=M^-J,\quad
J=\begin{pmatrix}1-a b&a e^{i\theta}\\-b e^{-i\theta}&1\end{pmatrix},
\quad\det J=1,\quad M=I+M_1/k+O(k^{-2}).}
$$

The data $a,b$ are time-independent in this convention; their spatial and temporal oscillations are displayed explicitly. Setting $b=0$ and $a=\widehat q_0$ recovers the linear problem. Thus the diagonal correction $-ab$ is necessary when the second off-diagonal jump is introduced; omitting it would destroy [determinant](../../../../../determinant.md) one.

To verify the deformation rather than merely name it, note $J_x=(ik/2)[D,J]$ and $J_t=-(ik^2/2)[D,J]$. Therefore $(M_x-(ik/2)[D,M])M^{-1}$ and $(M_t+(ik^2/2)[D,M])M^{-1}$ have no jump. Analyticity and the expansion at infinity make them, by Liouville's theorem, respectively $Q$ and $-kQ+V_0$. The first expansion gives $Q=-(i/2)[D,M_1]$, so

$$
q=-i(M_1)_{12},\qquad\vartheta=i(M_1)_{21}.
$$

The constant term of the second expression is $V_0=(M_1)_x$. In the first equation's next coefficient, its off-diagonal part equals $iDQ_x$ and its diagonal part equals $-iDQ^2$. Hence $V_0=iD(Q_x-Q^2)$, exactly the displayed nonlinear [Lax pair](../../../../../lax-pair.md). This proves that the reconstructed functions obey the required PDEs.

Finally let $C$ be the Cauchy integral operator on the real axis, $C_-$ its lower boundary value, and $\mu=M^-$. The jump relation and normalization give

$$
\boxed{\mu=I+C_-[\mu(J-I)],\qquad
M=I+C[\mu(J-I)].}
$$

This is the requested linear singular integral equation for the inverse problem: it is linear in the unknown [matrix](../../../../../matrix.md) $\mu$ once the scattering data are given. Reconstruction is $q=(2\pi)^{-1}\int[\mu(J-I)]_{12}ds$ and $\vartheta=-(2\pi)^{-1}\int[\mu(J-I)]_{21}ds$.

For completeness, generic simple discrete [eigenvalues](../../../../../eigenvalue.md) add the following residue data. At an upper-half-plane pole $k_j$, use $C_j=\begin{pmatrix}0&c_je^{i\theta(k_j)}\\0&0\end{pmatrix}$; at a lower-half-plane pole use $C_j=\begin{pmatrix}0&0\\d_je^{-i\theta(k_j)}&0\end{pmatrix}$, with the norming constants determined by the initial spatial scattering problem. Impose $\operatorname{Res}_{k_j}M=\lim_{k\to k_j}M C_j$. The nilpotent [matrices](../../../../../matrix.md) make this limit well-defined. If $A_j$ denotes the residue, the full linear inverse system is

$$
\mu(s)=I+C_-[\mu(J-I)](s)+\sum_j\frac{A_j}{s-k_j},
\qquad
A_j=\left(I+C[\mu(J-I)](k_j)+\sum_{\ell\ne j}\frac{A_\ell}{k_j-k_\ell}\right)C_j.
$$

The reconstructed field formulas acquire $-i\sum_j(A_j)_{12}$ and $i\sum_j(A_j)_{21}$ respectively. This includes the [soliton](../../../../../soliton.md) terms when they occur; the preceding pure-jump formula is their pole-free special case. These standard scattering formulations assume no spectral singularity on the real contour and simple discrete [eigenvalues](../../../../../eigenvalue.md); repeated poles require the corresponding higher-order pole conditions.

## ↑ Ancestors (10)

1. [31E](../31e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
