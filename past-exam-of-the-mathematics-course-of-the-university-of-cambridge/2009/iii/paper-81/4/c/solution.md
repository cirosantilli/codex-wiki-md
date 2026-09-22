<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\sigma=0$ under the assumed stationary-onset hypothesis, and let $\kappa=h\kappa'$ with fixed nonzero $\kappa'$. Substitute $W=hW_0+h^2W_1+\cdots$, $N=N_0+hN_1+h^2N_2+\cdots$, and $R_c=h^{-1}(R_0+hR_1+\cdots)$ into the modal equations and plate [boundary conditions](../../../../../../boundary-condition.md).

At leading order the concentration equation is $N_0''=0$, with $N_0'=0$ at both plates. Normalize its nonzero constant to $N_0=1$. The first nonzero momentum equation is

$$
W_0''''=-\kappa'^2R_0,\qquad W_0=W_0'=0\quad(z=-1,0).
$$

Integrating four times and imposing all four clamped [boundary conditions](../../../../../../boundary-condition.md) gives

$$
\boxed{N_0=1,\qquad W_0=-\frac{\kappa'^2R_0}{24}z^2(z+1)^2.}
$$

At the next concentration order, $\bar n=1+O(h)$ and $\bar n'=h+O(h^2)$, so the vertical advection of the basic concentration does not yet contribute. Thus

$$
N_1''=-GW_0'',\qquad N_1'=N_0=1\quad(z=-1,0).
$$

Integration gives $N_1=-GW_0+z+C_1$. The constant $C_1$ is an amplitude-normalization freedom; set it to zero, obtaining

$$
\boxed{N_1=-GW_0+z.}
$$

There is no need to require zero depth average of this concentration [eigenfunction](../../../../../../eigenfunction.md): for a nonzero horizontal [wavenumber](../../../../../../wavenumber.md) the horizontal average is already zero.

Use $\bar n=1+h(z+1/2)+O(h^2)$ and $\bar n'=h+O(h^2)$. At order $h^2$, the concentration equation is

$$
N_2''-N_1'-\kappa'^2=W_0-GW_1''-G\left(z+\frac12\right)W_0''.
$$

The corresponding cell-flux [boundary conditions](../../../../../../boundary-condition.md) are $N_2'=N_1$ at both plates. Integrate the equation from $-1$ to zero. Its left derivative term satisfies

$$
N_2'(0)-N_2'(-1)=N_1(0)-N_1(-1)=\int_{-1}^0N_1'dz.
$$

The $N_1'$ terms therefore cancel. The no-slip conditions imply $\int W_1''dz=0$. Also [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_{-1}^0\left(z+\frac12\right)W_0''dz
=\left[\left(z+\frac12\right)W_0'-W_0\right]_{-1}^0=0.
$$

Consequently the [solvability condition](../../../../../../solvability-condition.md) is simply

$$
0=\kappa'^2+\int_{-1}^0W_0dz
=\kappa'^2\left(1-\frac{R_0}{720}\right),
$$

since $\int_{-1}^0z^2(z+1)^2dz=1/30$. For every fixed nonzero $\kappa'$, the [long-wave bioconvection threshold in weak stratification](../../../../../../long-wave-bioconvection-threshold-in-weak-stratification.md) is therefore

$$
\boxed{R_0=720,\qquad R_c\sim\frac{720}{h}.}
$$

The cancellation shows why $G$ does not enter this leading coefficient; neither does $S$ at stationary onset. In dimensional terms, the leading critical mean number density and volume fraction are

$$
\boxed{C_{0c}\sim\frac{720\rho\nu D^2}{gv\Delta\rho V_sH^4},\qquad \varphi_{0c}\sim\frac{720\rho\nu D^2}{g\Delta\rho V_sH^4}.}
$$

These assume heavier-than-fluid cells, $\Delta\rho>0$. Exactly $\kappa'=0$ makes the integrated equation identically zero and corresponds to a spatially uniform change of conserved cell number, not a convective mode; the statement independent of $\kappa'$ is interpreted for nonzero long waves or their limit. This is the leading threshold within the specified long-wave, real-[eigenvalue](../../../../../../eigenvalue.md) assumptions. It does not by itself rule out a different finite-wavelength or oscillatory instability outside those assumptions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
