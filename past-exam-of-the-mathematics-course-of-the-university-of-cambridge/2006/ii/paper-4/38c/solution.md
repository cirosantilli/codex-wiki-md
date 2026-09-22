<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

For a physical adiabatic [ideal gas](../../../../../ideal-gas.md) one has $\gamma>1$; the following algebra also holds for positive $\gamma\ne1$. Compression work implies $p=\rho W'(\rho)-W$, obtained by differentiating the total internal energy $VW(M/V)$ at fixed mass. With the stated pressure law this integrates to

$$
\boxed{W(\rho)=p/(\gamma-1)+C\rho}.
$$

The term proportional to mass is an arbitrary energy reference; set $C=0$. [Mass flux](../../../../../mass-flux.md) is $\rho u$, [momentum flux](../../../../../momentum-flux.md) is $p+\rho u^2$, and dividing the energy flux by [mass flux](../../../../../mass-flux.md) gives

$$
\boxed{\frac{\gamma}{\gamma-1}\frac p\rho+\frac{u^2}{2}=\text{constant}}
$$

for steady flow.

Work in the shock's rest frame. If the shock speed in the laboratory is $D$, upstream speed relative to it is $D$ and downstream speed is $D/r$, where $r=\rho_1/\rho_0$. Conservation of momentum gives $p_1-p_0=\rho_0D^2(1-1/r)$. Conservation of specific total enthalpy gives

$$
\frac\gamma{\gamma-1}\frac{p_0}{\rho_0}+\frac{D^2}{2}
=\frac\gamma{\gamma-1}\frac{p_1}{r\rho_0}+\frac{D^2}{2r^2}.
$$

Eliminating $D^2$ and using $p_1/p_0=1+\beta$ yields

$$
\boxed{\frac{\rho_1}{\rho_0}=\frac{2\gamma+(\gamma+1)\beta}{2\gamma+(\gamma-1)\beta}}.
$$

Its weak-shock expansion is $1+\beta/\gamma-(\gamma-1)\beta^2/(2\gamma^2)+O(\beta^3)$, exactly the expansion of $(1+\beta)^{1/\gamma}$ through second order. Thus the adiabatic pressure-density relation agrees to order $\beta^2$; [entropy](../../../../../entropy.md) production first affects this comparison at higher order. The same isentropic constant is not exactly preserved across a finite shock. The wording allows $\gamma=1$, but the printed enthalpy formula is then undefined. The compression calculation instead gives $W=(p_0/\rho_0)\rho\log(\rho/\rho_0)+C\rho$, and the [specific enthalpy](../../../../../specific-enthalpy.md) is $(p_0/\rho_0)[1+\log(\rho/\rho_0)]+C$. Thus the requested formula containing $1/(\gamma-1)$ requires $\gamma\ne1$; its physical ideal-gas application uses $\gamma>1$.

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
