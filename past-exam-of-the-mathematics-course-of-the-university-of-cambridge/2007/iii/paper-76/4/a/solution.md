<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the material-first [nominal stress tensor](../../../../../../nominal-stress-tensor.md) convention $P_{Ii}$, with $F_{iI}$ the [deformation gradient](../../../../../../deformation-gradient.md). For any fixed reference material subvolume $V_0$ with outward unit normal $N$, [conservation of energy](../../../../../../conservation-of-energy.md) is

$$
\frac d{dt}\int_{V_0}\rho_0\left(U+\frac12|v|^2\right)dV_0
=\int_{V_0}\rho_0(b\cdot v+r)\,dV_0+\int_{\partial V_0}\left[(P^TN)\cdot v-q\cdot N\right]dA_0.
$$

Here $b$ is [body force](../../../../../../body-force.md) per mass, $r$ is heat supply per mass and $q$ is nominal [heat flux](../../../../../../heat-flux-density.md). Using [momentum conservation](../../../../../../momentum-conservation.md) to remove the [kinetic energy](../../../../../../kinetic-energy.md) balance gives the integral [Lagrangian internal energy balance](../../../../../../lagrangian-internal-energy-balance.md):

$$
\frac d{dt}\int_{V_0}\rho_0U\,dV_0=\int_{V_0}(P_{Ii}\dot F_{iI}+\rho_0r)\,dV_0-\int_{\partial V_0}q_IN_I\,dA_0.
$$

The integral [Lagrangian entropy inequality](../../../../../../lagrangian-entropy-inequality.md) is

$$
\frac d{dt}\int_{V_0}\rho_0\eta\,dV_0\ge\int_{V_0}\frac{\rho_0r}{\theta}\,dV_0-\int_{\partial V_0}\frac{q_IN_I}{\theta}\,dA_0,
$$

where $\theta>0$ is [temperature](../../../../../../temperature.md) and $q/\theta$ is the [thermodynamic entropy flux](../../../../../../thermodynamic-entropy-flux.md).

Since the subvolume is arbitrary, the [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
\rho_0\dot U=P_{Ii}\dot F_{iI}+\rho_0r-q_{I,I},\qquad \rho_0\theta\dot\eta\ge\rho_0r-q_{I,I}+\frac{q_I\theta_{,I}}{\theta}.
$$

Expand $\dot U=U_{,F_{iI}}\dot F_{iI}+U_{,\eta}\dot\eta+U_{,\xi_r}\dot\xi_r$ and eliminate the heat supply between these relations. The [Clausius-Duhem inequality](../../../../../../clausius-duhem-inequality.md) becomes

$$
(P_{Ii}-\rho_0U_{,F_{iI}})\dot F_{iI}+\rho_0(\theta-U_{,\eta})\dot\eta-\rho_0U_{,\xi_r}\dot\xi_r-\frac{q_I\theta_{,I}}{\theta}\ge0.
$$

Under the usual local constitutive independence assumptions, the reversible mechanical and thermal variations can have either sign. The [Coleman-Noll procedure](../../../../../../coleman-noll-procedure.md) therefore imposes

$$
\boxed{P_{Ii}=\rho_0\frac{\partial U}{\partial F_{iI}},\qquad\theta=\frac{\partial U}{\partial\eta}.}
$$

Define the [thermodynamic force conjugate to an internal variable](../../../../../../thermodynamic-force-conjugate-to-an-internal-variable.md) by $f_r=-\rho_0U_{,\xi_r}$. The energy balance and the remaining entropy constraint now give, respectively,

$$
\boxed{\rho_0\theta\dot\eta=\rho_0r-q_{I,I}+f_r\dot\xi_r,\qquad f_r\dot\xi_r-\frac{q_I\theta_{,I}}{\theta}\ge0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
