# Entropy production by Fourier heat conduction

↑ **Parent:** [Thermal conduction](thermal-conduction.md)

For an [ideal gas](ideal-gas-split.md) with specific internal energy $c_vT$ and [Fourier's law](fourier-s-law.md) heat flux $\mathbf q=-k\nabla T$, subtraction of the kinetic-energy balance from total energy gives $\rho c_v DT/Dt+p\nabla\cdot\mathbf u=\nabla\cdot(k\nabla T)$. The [thermodynamic entropy](entropy-split.md) satisfies $TDS/Dt=c_vDT/Dt+p\nabla\cdot\mathbf u/\rho$, so

$$
\rho\frac{DS}{Dt}=\frac1T\nabla\cdot(k\nabla T)=\nabla\cdot\left(\frac{k\nabla T}{T}\right)+\frac{k|\nabla T|^2}{T^2}.
$$

The divergence describes entropy transport by heat; the final term is local irreversible production. For $T>0$ and $k\geq0$ it is nonnegative. In a fixed impermeable thermally insulated container, boundary entropy flux vanishes and mass conservation gives $d\int\rho S\,dV/dt=\int k|\nabla T|^2/T^2\,dV$. Insulation conserves total energy while permitting entropy to increase as temperature gradients relax.

## ↑ Ancestors (7)

1. [Thermal conduction](thermal-conduction.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-theoretical-mechanics-course-of-the-university-of-oxford/2008/b/5/solution.md)
