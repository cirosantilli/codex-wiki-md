<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrate any conservation equation from part (a) through a vanishingly thin control volume moving with shock speed $s$. Its singular terms require $[F]=s[Q]$. The stationary shock has $s=0$, so all five fluxes are continuous. Substitution gives the [Rankine-Hugoniot conditions for a perfect gas](../../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md):

$$
\boxed{[\rho v]=0,\quad[\rho v^2+p]=0,\quad
[\rho vu_y]=[\rho vu_z]=0,\quad
[\rho v(u^2/2+w)]=0.}
$$

Let the common mass flux be $j=\rho_1v_1=\rho_2v_2>0$. Dividing the transverse conditions by $j$ proves $u_{y2}=u_{y1}$ and $u_{z2}=u_{z1}$. Dividing the energy condition by $j$ shows that $u^2/2+w$ is unchanged. Thus tangential kinetic energies cancel when solving for the normal shock compression. No global equality of the [entropy](../../../../../../entropy.md) parameter $p/\rho^\gamma$ across the shock has been assumed: physical dissipative shocks increase that parameter.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
