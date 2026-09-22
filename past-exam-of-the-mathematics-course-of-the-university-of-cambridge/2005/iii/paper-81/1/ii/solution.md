<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Once $C$ is removed, the remaining connected segments form the chain $K\to L\to N\to M$, of total length $3\ell$. For $RY\gg1$, each [hydraulic resistance](../../../../../../hydraulic-resistance.md) draws a small flow, so to leading order the far end at $M$ is reflecting, with zero segment flow there. Successive [wave transfer matrices of an arterial segment](../../../../../../wave-transfer-matrix-of-an-arterial-segment.md) give

$$
p_N=\cos\beta\,p_M,\qquad p_L=\cos2\beta\,p_M,\qquad
p_K=\cos3\beta\,p_M,\qquad q_K=iY\sin3\beta\,p_M.
$$

The incident-plus-reflected inlet relation remains $q_K=2Y(2P_A-p_K)$. Therefore, defining $D=3e^{3i\beta}+e^{-3i\beta}$,

$$
\boxed{Q_M^{\rm blocked}\sim\frac{8P_A}{RD},\quad
Q_N^{\rm blocked}\sim\frac{8P_A\cos\beta}{RD},\quad
Q_L^{\rm blocked}\sim\frac{8P_A\cos2\beta}{RD}.}
$$

The modulus of $D$ equals $\gamma=|3e^{4i\beta}+e^{-2i\beta}|$, because the expressions differ by a unit-modulus factor. Comparison with the normal flows gives the amplitude ratios

$$
\boxed{\frac{|Q_N^{\rm blocked}|}{|Q_N^{\rm normal}|}\sim\frac{4|\cos\beta|}{\gamma},\qquad
\frac{|Q_M^{\rm blocked}|}{|Q_M^{\rm normal}|}\sim\frac4{\gamma|\cos\beta|},\qquad
\frac{|Q_L^{\rm blocked}|}{|Q_L^{\rm normal}|}\sim\frac{4|\cos2\beta|}{\gamma|\cos\beta|}.}
$$

For small phases the cosines are positive and the absolute values can be removed. The original PDF prints an additional $\cos(\beta/2)$ in the middle numerator. That factor does not follow from the displayed equal-length network: the transfer relation from $M$ to $K$ above fixes $p_M=8P_A/D$, with no such factor. The corrected middle ratio is shown here.

Since $\gamma^2=10+6\cos6\beta$, one has $\gamma=4[1-27\beta^2/8+O(\beta^4)]$. Thus the three corrected ratios, in the order $N,M,L$, are

$$
1+\frac{23}{8}\beta^2+O(\beta^4),\qquad
1+\frac{31}{8}\beta^2+O(\beta^4),\qquad
1+\frac{15}{8}\beta^2+O(\beta^4).
$$

**All three exceed one for sufficiently small nonzero $\beta$; they equal one at zero [frequency](../../../../../../frequency.md).** This is an oscillatory [arterial wave reflection](../../../../../../reflection-of-an-arterial-pressure-wave.md) effect, not an increase in steady conductance. Removing a branch changes the [standing wave](../../../../../../standing-wave.md) pattern and the total inlet [pressure](../../../../../../pressure.md) associated with a fixed incident wave. Reflected waves can enhance junction [pressures](../../../../../../pressure.md) and hence peripheral flow amplitudes. Neither total inlet [pressure](../../../../../../pressure.md) nor total inlet flow was held fixed, and no extra energy source is implied.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
