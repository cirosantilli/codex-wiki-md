<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

The [Maxwell equations](../../../../../maxwell-equations.md) with vacuum permittivity and permeability give $\rho=\epsilon_0\nabla\cdot E$ and $J=\mu_0^{-1}\nabla\times B-\epsilon_0\partial_tE$. The current identity is the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md), and [Faraday's law](../../../../../faraday-s-law-of-induction.md) gives $\partial_tB=-\nabla\times E$. With $g=\epsilon_0E\times B$,

$$
 f+\partial_tg=\epsilon_0[(\nabla\cdot E)E-E\times(\nabla\times E)]+
 \mu_0^{-1}(\nabla\times B)\times B.
$$

The identity $(\nabla\times B)\times B=(B\cdot\nabla)B-\tfrac12\nabla B^2$, and its electric analogue, turn this into the divergence of the [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md) $T$. Thus the tensor in the question is its negative:

$$
\boxed{\sigma_{ij}=\epsilon_0\left(\frac12E^2\delta_{ij}-E_iE_j\right)
 +\frac1{\mu_0}\left(\frac12B^2\delta_{ij}-B_iB_j\right),\qquad
 \partial_tg_i+\partial_j\sigma_{ij}=-f_i.}
$$

The [vector](../../../../../vector.md) $g$ is [electromagnetic momentum density](../../../../../electromagnetic-momentum-density.md), and $\sigma_{ij}$ is the outward flux of its $i$th component across a surface normal in the $j$ direction. In static conditions the total [force](../../../../../force.md) on matter is $F_i=-\oint\sigma_{ij}n_j\,dS$; generally subtract the time [derivative](../../../../../derivative.md) of the enclosed [electromagnetic field](../../../../../electromagnetic-field.md) [momentum](../../../../../momentum.md) as well.

For the two infinite sheets, superposition and the [electromagnetic field](../../../../../electromagnetic-field.md) jumps give $E=(\sigma/\epsilon_0)e_x$, $B=\mu_0K e_y$ between them and zero outside. Substitution yields exactly

$$
 \sigma_{ij}=\frac{\sigma^2}{2\epsilon_0}\operatorname{diag}(-1,1,1)
 +\frac{\mu_0K^2}{2}\operatorname{diag}(1,-1,1).
$$

A thin pillbox enclosing the $x=0$ sheet has only its $+x$ face in the interior [electromagnetic field](../../../../../electromagnetic-field.md). Therefore

$$
\boxed{\frac FA=\left(\frac{\sigma^2}{2\epsilon_0}-\frac{\mu_0K^2}{2}\right)e_x.}
$$

Directly, omit the sheet's self-[electromagnetic field](../../../../../electromagnetic-field.md): the other sheet supplies $E_{\rm other}=\sigma e_x/(2\epsilon_0)$ and $B_{\rm other}=\mu_0K e_y/2$. The [Lorentz force](../../../../../lorentz-force.md) per area is $\sigma E_{\rm other}+K e_z\times B_{\rm other}$, giving the same result. The electric contribution is attractive and the magnetic contribution repulsive.

If $K=\sigma v$ for a single moving charge population, use $\mu_0\epsilon_0=c^{-2}$ to obtain $F/A=\sigma^2(1-v^2/c^2)e_x/(2\epsilon_0)$. For physical $|v|<c$ this is attractive, so **motion of these charges cannot make the [force](../../../../../force.md) repulsive**. Independently imposed currents need not satisfy that restriction on $K/\sigma$.

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
