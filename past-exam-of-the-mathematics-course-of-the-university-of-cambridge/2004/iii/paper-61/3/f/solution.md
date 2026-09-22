<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

We derive the Robin spectral elimination while retaining the finite-time [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md). This distinguishes the actual ratio $B/A$ from the equivalent, time-independent boundary coefficient needed by the [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md).

At $x=0$ the time [Lax pair](../../../../../../lax-pair.md) coefficient has off-diagonal entries $(2k+ic)q$ and $(2k-ic)\bar q$. Let

$$
K(k)=\operatorname{diag}(2k+ic,-2k+ic),\qquad h(k)=\frac{2k-ic}{2k+ic}.
$$

Direct multiplication shows $V(0,t,k)=K(k)V(0,t,-k)K(k)^{-1}$. Because the commutator term depends on $k^2$ and $K$ commutes with $\sigma_3$, uniqueness of the time [Volterra integral equation](../../../../../../volterra-integral-equation.md) gives $S(k)=K(k)S(-k)K(k)^{-1}$. Therefore

$$
\boxed{A(-k)=A(k),\qquad B(-k)=-h(k)B(k).}
$$

The exceptional parameter points of $K$ are treated by analytic continuation. These identities express [linearizable Robin scattering for defocusing NLS](../../../../../../linearizable-robin-scattering-for-defocusing-nls.md).

For finite horizon $T$, the exact upper-half-plane ratio is

$$
\frac{B(k;T)}{A(k;T)}=\frac{b(k)}{a(k)}-\frac{e^{4ik^2T}c_T(k)}{a(k)A(k;T)}.
$$

Consequently the often used answer $B/A=b/a$ is not a literal finite-$T$ identity. Its effective time-independent replacement, in the two bounded time sectors, is

$$
\boxed{\widetilde R(k)=\begin{cases}b(k)/a(k),&k\in D_1,\\-\dfrac{2k+ic}{2k-ic}\dfrac{b(-k)}{a(-k)},&k\in D_3.\end{cases}}
$$

The second branch follows from the Robin symmetry; its argument $-k$ lies in the upper half-plane where the initial scattering functions are known. We now justify this replacement for the inverse problem without assuming that boundary values decay as $t\to\infty$.

Only $\Gamma=B^\sharp/(ad)$ is needed for the connection across the upper imaginary ray. The conjugate [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) at $-k$ and the Robin symmetry give

$$
\frac{B^\sharp(k)}{A^\sharp(k)}=-h(k)\frac{b^\sharp(-k)}{a^\sharp(-k)}+h(k)e^{-4ik^2T}\frac{c_T^\sharp(-k)}{a^\sharp(-k)A^\sharp(k)}.
$$

For upper-half-plane $k$, the notation $b^\sharp(-k)=\overline{b(-\bar k)}$ uses only values of $b$ in its legitimate upper-half-plane domain. Put

$$
\Delta(k)=a(k)a^\sharp(-k)+h(k)b(k)b^\sharp(-k),\qquad\mathcal D(k)=(2k+ic)\Delta(k).
$$

The effective boundary coefficient is

$$
\boxed{\widetilde\Gamma(k)=-\frac{h(k)b^\sharp(-k)}{a(k)\Delta(k)}=-\frac{(2k-ic)b^\sharp(-k)}{a(k)\mathcal D(k)}.}
$$

This [Robin spectral determinant for defocusing NLS](../../../../../../robin-spectral-determinant-for-defocusing-nls.md) is explicitly computed from the initial data and $c$.

For completeness, the finite-horizon defect can be removed algebraically, not by an unproved limit. If $r=B^\sharp/A^\sharp$, then $\Gamma=r/[a(a-br)]$. Subtracting the same expression with $r_0=-h b^\sharp(-k)/a^\sharp(-k)$ gives

$$
\Gamma-\widetilde\Gamma=\frac{h(k)e^{-4ik^2T}c_T^\sharp(-k)}{d(k)\Delta(k)}.
$$

Its jump multiplier is

$$
(\Gamma-\widetilde\Gamma)e^{2i\theta}=\frac{h(k)c_T^\sharp(-k)}{d(k)\Delta(k)}e^{2ikx-4ik^2(T-t)}.
$$

The exponential decays in $D_2$ for $x>0$ and $t<T$, since $\operatorname{Im}k>0$ and $\operatorname{Im}k^2<0$. The coefficient is holomorphic away from the stated determinant zeros and is appropriately decaying at infinity. From the explicit matrices in part (c), $C_2=C_1L(\Gamma e^{2i\theta})$, where $L(z)=\begin{pmatrix}1&0\\z&1\end{pmatrix}$. Hence replace the sector-two solution by

$$
\widetilde M_2=M_2L\bigl((\widetilde\Gamma-\Gamma)e^{2i\theta}\bigr).
$$

The reflected upper-triangular change is made in $D_3$. These analytic changes remove the finite-time defect, leave $M_1,M_4$ unchanged, and leave the reconstruction from the second column in $D_2$ unchanged. At apparent poles, the old $d$-dependent singularities cancel by the connection formula; genuine poles of the new determinant remain as explicit residue data. Equivalently, small circles can first isolate all zeros and the same algebra can be performed on the regularized contours. This is [finite-horizon Robin spectral elimination](../../../../../../finite-horizon-robin-spectral-elimination.md).

Every modified jump is now explicitly known: keep $C_1,C_4$ from part (c) and replace

$$
C_2\longmapsto C_1L(\widetilde\Gamma e^{2i\theta}),\qquad C_3\longmapsto C_4U(\widetilde\Gamma^\sharp e^{-2i\theta}),\qquad U(z)=\begin{pmatrix}1&z\\0&1\end{pmatrix}.
$$

All jumps are again $C_-^{-1}C_+$, now involving only $a,b,c$. If $\mathcal D$ has a simple zero $k_j$ giving a genuine pole, its coefficient is

$$
\gamma_j=-\frac{(2k_j-ic)b^\sharp(-k_j)}{a(k_j)\mathcal D'(k_j)},\qquad\operatorname*{Res}_{k=k_j}[\widetilde M]_1=\gamma_je^{2i\theta(k_j)}[\widetilde M(k_j)]_2,
$$

with the reflected second-column condition at $\bar k_j$. Common numerator/denominator zeros are checked for removability, and zeros on the cross require contour indentation or local circle jumps. Thus no unknown boundary norming data remain. One must not assume away such zeros for every real $c$; attractive Robin parameters can support localized modes.

It follows that **the equivalent normalized Riemann-Hilbert problem is specified entirely by $q_0$ and $c$**, including its pole data. When two solutions exist, their quotient has no jump, its prescribed pole singularities cancel, and it tends to $I$ at infinity; [Liouville theorem](../../../../../../liouville-theorem.md) makes the quotient $I$, proving uniqueness. Smooth corner evolution additionally requires $q_0'(0)=cq_0(0)$ and higher compatibility conditions at higher regularity. Without that compatibility, the same initial data are interpreted in the weak evolution sense, rather than as a smooth solution through the corner.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
