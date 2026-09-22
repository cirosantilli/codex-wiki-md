<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $|0\rangle=|\uparrow\rangle$, $|1\rangle=|\downarrow\rangle$, and use $X_j,Y_j$ for the [Pauli matrices](../../../../../pauli-matrices.md) on particle $j$. Their actions on the [computational basis](../../../../../computational-basis.md) are

$$
X|0\rangle=|1\rangle,\quad X|1\rangle=|0\rangle,\quad Y|0\rangle=i|1\rangle,\quad Y|1\rangle=-i|0\rangle.
$$

Set $P_1=X_1Y_2Y_3$, $P_2=Y_1X_2Y_3$, $P_3=Y_1Y_2X_3$, and $P_4=X_1X_2X_3$. Any two distinct operators in this list differ by an $X$ versus $Y$ at exactly two sites. At each such site $XY=-YX$, while factors on different particles commute. Swapping the two full products therefore introduces two minus signs, giving

$$
\boxed{[P_i,P_j]=0\quad\text{for every }i,j.}
$$

This is the [Pauli-string commutation parity](../../../../../pauli-string-commutation-parity.md) rule. Each product is Hermitian and squares to the identity, so its only [eigenvalues](../../../../../eigenvalue.md) are $\pm1$.

For the negative-phase [Greenberger–Horne–Zeilinger state](../../../../../greenberger-horne-zeilinger-state.md), put $|G_-\rangle=(|000\rangle-|111\rangle)/\sqrt2$. The two $Y$ factors in each of $P_1,P_2,P_3$ contribute $i^2=-1$ on $|000\rangle$ and $(-i)^2=-1$ on $|111\rangle$. Thus these operators take $|000\rangle$ to $-|111\rangle$ and $|111\rangle$ to $-|000\rangle$. By contrast, $P_4$ flips these two basis states without a phase. Consequently

$$
\boxed{P_1|G_-\rangle=P_2|G_-\rangle=P_3|G_-\rangle=|G_-\rangle,\qquad P_4|G_-\rangle=-|G_-\rangle.}
$$

The [GHZ state](../../../../../greenberger-horne-zeilinger-state.md) is therefore a simultaneous eigenstate of the four commuting products. As a sign check, direct multiplication gives

$$
P_1P_2P_3=(XYY)_1(YXY)_2(YYX)_3=-X_1X_2X_3=-P_4.
$$

This is compatible with the displayed quantum [eigenvalues](../../../../../eigenvalue.md).

Now apply the [EPR criterion of reality](../../../../../epr-criterion-of-reality.md) together with locality for the spacelike separated particles. In the context with local settings $X_1,Y_2,Y_3$, the product of the three outcomes is certainly $+1$. Therefore the two remote $Y$ outcomes predict the first particle's $X$ outcome with certainty, without disturbing it under the locality assumption. The other perfect-correlation contexts similarly predict each particle's $X$ or $Y$ outcome from measurements performed only on the other particles. The [EPR criterion of reality](../../../../../epr-criterion-of-reality.md) then assigns predetermined local values $x_j,y_j\in\{+1,-1\}$ to these six observables. Locality makes the value assigned at one site independent of which measurements were chosen at the other sites.

To reproduce the three certain mixed-setting quantum predictions, every such assignment must satisfy

$$
x_1y_2y_3=1,\qquad y_1x_2y_3=1,\qquad y_1y_2x_3=1.
$$

Multiplying these scalar equations cancels each squared $y_j$ and gives $x_1x_2x_3=+1$. But the all-$X$ quantum prediction, from the $P_4$ eigenvalue, is $x_1x_2x_3=-1$ with certainty. Hence

$$
\boxed{\text{local EPR assignments predict }+1,\qquad\text{quantum mechanics predicts }-1.}
$$

**The perfect GHZ correlations contradict the simultaneous local elements of reality inferred by the EPR argument.** No statistical Bell inequality is needed. The locality assumption is essential to that inference; the certainty criterion without the premise that distant choices cannot disturb the local element does not by itself imply a local hidden-variable model. Nor does the argument require simultaneous measurement of $X$ and $Y$ on a single particle: different experimental contexts establish the perfect predictions, and it is the EPR/locality interpretation that attempts to assign all their values at once.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
