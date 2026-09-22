<h1 id="1/iii/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

All free indices below are spatial, and $K=\gamma^{\mu\nu}K_{\mu\nu}$. Contract the vacuum [Ricci tensor](../../../../../../../ricci-tensor.md) using $g^{\mu\nu}=\gamma^{\mu\nu}-n^\mu n^\nu$:

$$
0=(\perp R_{\alpha\beta})
=\gamma^{\mu\nu}(\perp R)_{\mu\alpha\nu\beta}
-n^\mu n^\nu R_{\mu\alpha\nu\beta}.
$$

Reversing both antisymmetric curvature pairs identifies the last term as $-E_{\alpha\beta}$. The spatial [Gauss–Codazzi equations for a spatial hypersurface](../../../../../../../gauss-codazzi-equations-for-a-spatial-hypersurface.md) then give

$$
E_{\alpha\beta}
=\gamma^{\mu\nu}\bigl(\mathcal R_{\mu\alpha\nu\beta}
+K_{\mu\nu}K_{\beta\alpha}-K_{\mu\beta}K_{\nu\alpha}\bigr)
=\mathcal R_{\alpha\beta}+KK_{\alpha\beta}-K^\nu{}_\beta K_{\nu\alpha}.
$$

For the [magnetic part of the Weyl tensor](../../../../../../../magnetic-part-of-the-weyl-tensor.md), moving the normal to the first slot of the [metric volume tensor](../../../../../../../metric-volume-tensor.md) introduces a minus sign:

$$
\epsilon_{\alpha\lambda\mu\nu}n^\lambda=-\tilde\epsilon_{\alpha\mu\nu}.
$$

The remaining curvature indices are spatial, so the normal projection in the [Gauss–Codazzi equations for a spatial hypersurface](../../../../../../../gauss-codazzi-equations-for-a-spatial-hypersurface.md) gives

$$
\begin{aligned}
B_{\alpha\beta}
&=-\frac12\tilde\epsilon_\alpha{}^{\mu\nu}R_{\mu\nu\beta\rho}n^\rho\\
&=-\frac12\tilde\epsilon_\alpha{}^{\mu\nu}(-D_\mu K_{\nu\beta}+D_\nu K_{\mu\beta})\\
&=\tilde\epsilon_\alpha{}^{\mu\nu}D_\mu K_{\nu\beta}.
\end{aligned}
$$

The interchange $\mu\leftrightarrow\nu$ makes the two [spatial covariant derivative](../../../../../../../spatial-covariant-derivative.md) terms equal. Thus **the constants, with the paper's orientation and extrinsic-curvature convention, are**

$$
\boxed{(k_1,k_2,k_3,k_4)=(1,1,-1,1).}
$$

In particular, the sign of the magnetic expression must include the minus from moving $n$ past the first volume-tensor index. These formulas reconstruct the spatial [electric part of the Weyl tensor](../../../../../../../electric-part-of-the-weyl-tensor.md) and [magnetic part of the Weyl tensor](../../../../../../../magnetic-part-of-the-weyl-tensor.md) from the [induced metric](../../../../../../../induced-metric.md) and the [extrinsic curvature of a spatial hypersurface](../../../../../../../extrinsic-curvature-of-a-spatial-hypersurface.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Iii](../../iii.md)
3. [1](../../../1.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
