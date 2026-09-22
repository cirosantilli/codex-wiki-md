<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With constant detected rates, $Q=R_QT$, $B=R_BT$. Squaring the previous [signal-to-noise ratio in photon counting](../../../../../../../signal-to-noise-ratio-in-photon-counting.md) gives

$$
R_Q^2T^2-Z^2(R_Q+2R_B)T-2nZ^2r^2=0.
$$

For $R_Q>0$, nonnegative background and target $Z>0$, choose the positive root:

$$
\boxed{T=\frac{Z^2(R_Q+2R_B)+\sqrt{Z^4(R_Q+2R_B)^2+8nR_Q^2Z^2r^2}}{2R_Q^2}.}
$$

The other root is nonpositive. With no [read noise](../../../../../../../read-noise.md), this reduces to $T=Z^2(R_Q+2R_B)/R_Q^2$; in a read-dominated short exposure it approaches $Z\sqrt{2n}\,r/R_Q$. If $R_Q=0$, no positive target stellar signal-to-noise is attainable. A zero target can be assigned zero exposure, with its limiting interpretation when all noise terms also vanish. Real [quantum efficiency](../../../../../../../quantum-efficiency.md) or multiple reads modifies the rates or read-variance term before solving the quadratic.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
