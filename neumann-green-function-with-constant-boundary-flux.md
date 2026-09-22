# Neumann Green function with constant boundary flux

↑ **Parent:** [Green's function](green-s-function-split.md)

For a smooth bounded connected [domain](domain-mathematical-analysis.md) $V$ with boundary $S$, integrating the [Green function](green-s-function-split.md) equation and applying the [divergence theorem](divergence-theorem.md) forces $\int_S\partial_nG\,dS=1$. Thus zero [Neumann boundary data](neumann-boundary-data.md) are incompatible with an unmodified unit point source. The displayed constant boundary derivative has the required total flux. For $\Delta\Phi=\sigma$ and $\partial_n\Phi=f$, the compatibility condition is $\int_V\sigma\,dV=\int_Sf\,dS$. [Green's second identity](green-second-identity.md) then yields

$$
\Phi(x_0)=\int_VG(x,x_0)\sigma(x)dV-\int_SG(x,x_0)f(x)dS+\frac1{|S|}\int_S\Phi\,dS.
$$

The last term is an undetermined additive constant. Adding a constant to $G$ does not change the other two terms together, because of the compatibility condition. This construction keeps the unit [Dirac delta](dirac-delta-function.md) source; using a mean-subtracted source with zero normal derivative is a different normalization.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/2/solution.md)
