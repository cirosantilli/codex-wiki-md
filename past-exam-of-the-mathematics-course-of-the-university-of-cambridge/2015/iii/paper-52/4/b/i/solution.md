<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the connection convention $\nabla_\alpha Y^\rho=\partial_\alpha Y^\rho+\Gamma^\rho{}_{\mu\alpha}Y^\mu$, with the derivative index last. This is consistent with the printed curvature formula and the final formula in part (iv). The paper's $T_{\mu\nu}{}^\rho=\Gamma^\rho{}_{\mu\nu}-\Gamma^\rho{}_{\nu\mu}$ is then the negative of the geometric [torsion tensor](../../../../../../../torsion-tensor.md) defined by $\mathcal T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]$. Keep the paper's component convention throughout this question.

Set $A_{\mu\nu\rho}=g_{\rho\lambda}(\Gamma^\lambda{}_{\mu\nu}-S^\lambda{}_{\mu\nu})$. The [difference of affine connections is a tensor](../../../../../../../difference-of-affine-connections-is-a-tensor.md). Since the [Levi-Civita connection](../../../../../../../levi-civita-connection.md) $S$ is symmetric and metric compatible, expanding the [nonmetricity tensor](../../../../../../../nonmetricity-tensor.md) gives

$$
T_{\mu\nu\rho}=A_{\mu\nu\rho}-A_{\nu\mu\rho},\qquad
N_{\mu\nu\rho}=-A_{\mu\rho\nu}-A_{\nu\rho\mu}.
$$

Here $T_{\mu\nu\rho}=g_{\rho\lambda}T_{\mu\nu}{}^\lambda$ is antisymmetric in its first two slots, while $N_{\mu\nu\rho}$ is symmetric in its first two slots. Cyclically permuting these identities and eliminating the other components gives

$$
A_{\mu\nu\rho}=\frac12\left(T_{\mu\nu\rho}+T_{\nu\rho\mu}-T_{\rho\mu\nu}
+N_{\mu\nu\rho}-N_{\nu\rho\mu}-N_{\rho\mu\nu}\right).
$$

Raise the last slot to obtain **the connection decomposition**

$$
\boxed{\Gamma^\rho{}_{\mu\nu}=S^\rho{}_{\mu\nu}-K_{\mu\nu}{}^\rho+W_{\mu\nu}{}^\rho,}
$$

where

$$
K_{\mu\nu}{}^\rho=-\frac12\left(T_{\mu\nu}{}^\rho+T_\nu{}^\rho{}_\mu-T^\rho{}_{\mu\nu}\right),\qquad
W_{\mu\nu}{}^\rho=\frac12\left(N_{\mu\nu}{}^\rho-N_\nu{}^\rho{}_\mu-N^\rho{}_{\mu\nu}\right).
$$

**The PDF is missing the factor $1/2$ in its definition of $K$.** With the printed $K$, the decomposition would instead contain $-K/2$. In these formulas $T^\rho{}_{\mu\nu}$ raises the first slot of the fully lowered [tensor](../../../../../../../tensor.md); it must not be confused with $T_{\mu\nu}{}^\rho$, which raises the last slot.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 52](../../../../paper-52-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
