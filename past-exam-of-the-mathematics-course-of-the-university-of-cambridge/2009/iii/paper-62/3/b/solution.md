<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To distinguish the moment quantity from the [gravitational constant](../../../../../../gravitational-constant.md), write it as $\mathcal G=\sum_i\boldsymbol p_i\cdot\boldsymbol r_i$. Newton's equations give $\dot{\boldsymbol p}_i=\boldsymbol F_i$ and $\dot{\boldsymbol r}_i=\boldsymbol p_i/m_i$. Differentiating proves

$$
\boxed{\frac{d\mathcal G}{dt}=\sum_i\frac{p_i^2}{m_i}+\sum_i\boldsymbol F_i\cdot\boldsymbol r_i
=2T+\sum_i\boldsymbol F_i\cdot\boldsymbol r_i.}
$$

Average from $0$ to $\tau$, divide by $\tau$, and apply the supplied long-time boundary condition. The result is

$$
0=2\langle T\rangle+\left\langle\sum_i\boldsymbol F_i\cdot\boldsymbol r_i\right\rangle,
\qquad\boxed{2\langle T\rangle=-\left\langle\sum_i\boldsymbol F_i\cdot\boldsymbol r_i\right\rangle.}
$$

The PDF's intermediate formula omits this minus sign. It cannot follow from the preceding derivative identity: an attractive inverse-square circular orbit already has $\boldsymbol F\cdot\boldsymbol r<0$ and $T>0$, contradicting the printed positive-sign version. The later homogeneous-potential relation is consistent with the corrected sign.

Interpret $W$ as the total pair [potential energy](../../../../../../potential-energy.md), with each pair counted once, for example $W=\sum_{i<j}C|\boldsymbol r_i-\boldsymbol r_j|^{p+1}$. The printed pair sum leaves one particle index unspecified; an ordered-pair convention with the corresponding factor absorbed into $C$ has the same degree of homogeneity. Under a common dilation of all positions,

$$
W(\lambda\boldsymbol r_1,\ldots,\lambda\boldsymbol r_N)=\lambda^{p+1}W(\boldsymbol r_1,\ldots,\boldsymbol r_N).
$$

Differentiating with respect to $\lambda$ at one is the [Euler theorem for homogeneous functions](../../../../../../euler-theorem-for-homogeneous-functions.md). Since $\boldsymbol F_i=-\nabla_iW$, it gives

$$
\sum_i\boldsymbol F_i\cdot\boldsymbol r_i=-(p+1)W.
$$

Substitution into the correctly signed averaged identity proves the [virial theorem for a homogeneous pair potential](../../../../../../virial-theorem-for-a-homogeneous-pair-potential.md):

$$
\boxed{2\langle T\rangle-(p+1)\langle W\rangle=0.}
$$

For $p\ne-1$, the conserved total [energy](../../../../../../energy.md) can be evaluated using these averages:

$$
E_{\rm tot}=\langle T\rangle+\langle W\rangle
=\frac{p+3}{p+1}\langle T\rangle.
$$

Use the kinetic [temperature](../../../../../../temperature.md) convention $\langle T\rangle=\kappa\Theta$, where $\kappa=3Nk_B/2>0$ for three-dimensional thermalized particles, or the same positive coefficient as a kinetic-temperature definition. At fixed particle number and interaction parameters,

$$
\frac{dE_{\rm tot}}{d\Theta}=\kappa\frac{p+3}{p+1}.
$$

Thus the equilibrium [heat capacity](../../../../../../heat-capacity.md) is negative precisely when

$$
\boxed{-3<p<-1,}
$$

subject to existence of the bounded equilibrium sequence assumed by the [virial theorem](../../../../../../virial-theorem.md). At $p=-3$ the virial energy is zero and this derivative vanishes. At $p=-1$ the written power-law potential is constant, its force vanishes, and the bounded-motion virial condition excludes nonzero kinetic energy; division by $p+1$ is not permissible. The Newtonian case $p=-2$ recovers $E_{\rm tot}=-\langle T\rangle$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
