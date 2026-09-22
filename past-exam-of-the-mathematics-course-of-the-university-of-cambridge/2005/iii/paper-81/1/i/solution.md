<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take positive [volumetric flow rate](../../../../../../volumetric-flow-rate.md) in the direction of increasing $x$. For an [arterial pressure wave](../../../../../../arterial-pressure-wave.md), the [characteristic admittance of an arterial wave](../../../../../../characteristic-admittance-of-an-arterial-wave.md) gives

$$
\boxed{q_B=Y(P_BE^--P_{BR}E^+).}
$$

The backward wave contributes the opposite flow sign. Write $p_j$ for each junction's complex [pressure](../../../../../../pressure.md) amplitude, suppressing the common $e^{i\omega t}$ factor, and put $r=RY$, $C_\beta=\cos\beta$, $S_\beta=\sin\beta$. The topology is the two paths $K\to L\to N$ and $K\to M\to N$; their intermediate and common distal junctions each have a [hydraulic resistance](../../../../../../hydraulic-resistance.md). The coordinate convention in the source puts the upstream end at $-\ell$ and the downstream end at zero in each segment. Consequently the [wave transfer matrix of an arterial segment](../../../../../../wave-transfer-matrix-of-an-arterial-segment.md) is

$$
\begin{pmatrix}p_u\\q_u\end{pmatrix}
=\begin{pmatrix}C_\beta&iS_\beta/Y\\iYS_\beta&C_\beta\end{pmatrix}
\begin{pmatrix}p_d\\q_d\end{pmatrix}.
$$

Equivalently $q_u=Y(C_\beta p_u-p_d)/(iS_\beta)$ and $q_d=Y(p_u-C_\beta p_d)/(iS_\beta)$, with their continuous limits understood when $S_\beta=0$.

Symmetry gives $p_L=p_M=p_s$. Distal [mass conservation](../../../../../../mass-conservation.md) and the resistive relation $Q_N=p_N/R$ give

$$
2\frac{Y}{iS_\beta}(p_s-C_\beta p_N)=\frac{p_N}{R},\qquad
p_s=\left(C_\beta+\frac{iS_\beta}{2r}\right)p_N.
$$

At $L$, the incoming flow supplies both its bed and segment $D$, so

$$
p_K=\left(2C_\beta+\frac{iS_\beta}{r}\right)p_s-p_N.
$$

Choose the incident amplitude $P_A$ at $K$. If $P_{AR}$ is the reflected amplitude in vessel $A$, [pressure](../../../../../../pressure.md) [continuity equation](../../../../../../continuity-equation.md) gives $p_K=P_A+P_{AR}$, while inlet flow is $2Y(P_A-P_{AR})=2Y(2P_A-p_K)$. Equating this to the two outgoing segment flows yields

$$
p_s=e^{i\beta}p_K-2iS_\beta P_A.
$$

Eliminating $p_s,p_K$ from these three relations gives the [wave transmission through a resistively loaded arterial loop](../../../../../../wave-transmission-through-a-resistively-loaded-arterial-loop.md) result

$$
\boxed{Q_N=P_A RY^2\frac{8e^{-i\beta}}{e^{i\beta}(2RY+1)^2+e^{-i\beta}(2RY-1)}.}
$$

For large $r$ at fixed phase, $p_N=2P_Ae^{-2i\beta}+O(r^{-1})$ and $p_M=C_\beta p_N+O(r^{-1})$. Hence

$$
\boxed{Q_N\sim\frac{2P_A}{R}e^{-2i\beta},\qquad Q_M=Q_L\sim\frac{2P_A}{R}e^{-2i\beta}\cos\beta.}
$$

These leading terms must not be used as nonzero denominators near a phase at which the normal intermediate flow vanishes.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
