<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Relaxation-time model.** The [Drude model](../../../drude-model.md) treats mobile charge carriers as independent particles accelerated by the [Lorentz force](../../../lorentz-force.md) between scattering events. Collisions randomize the drift [momentum](../../../momentum-split.md) toward local equilibrium and are represented by a uniform, field-independent [momentum relaxation time](../../../momentum-relaxation-time.md). For the present calculation the [carrier density](../../../carrier-density.md), isotropic [mass](../../../mass.md) and [relaxation time](../../../relaxation-time.md) are fixed, the fields are uniform and stationary, and quantum orbital quantization and intercarrier correlations are neglected. The steady [drift velocity](../../../drift-velocity.md) obeys

$$
0=q(\mathbf E+\mathbf v\times\mathbf B)-\frac m\tau\mathbf v.
$$

Here $n$ is the number of carriers of that species per unit volume, $q$ their **signed** charge, $m>0$ their inertial or isotropic band [mass](../../../mass.md), $\tau$ the [momentum relaxation time](../../../momentum-relaxation-time.md), and $\sigma_0$ their single-species [electrical conductivity](../../../electrical-conductivity.md) at zero field.

**One-carrier [tensor](../../../tensor.md).** With $\mathbf B=B\hat{\mathbf z}$ and $\mathbf J=nq\mathbf v$, solving for the [electric field](../../../electric-field-split.md) gives

$$
\mathbf E=\frac{m}{nq^2\tau}\mathbf J-\frac1{nq}\mathbf J\times\mathbf B.
$$

Since $(\mathbf J\times\mathbf B)_x=BJ_y$ and $(\mathbf J\times\mathbf B)_y=-BJ_x$,

$$
E_x=\frac{m}{nq^2\tau}J_x-\frac{B}{nq}J_y,\qquad E_y=\frac{B}{nq}J_x+\frac{m}{nq^2\tau}J_y.
$$

Thus the [resistivity tensor](../../../resistivity-tensor.md), defined by $\mathbf E=\boldsymbol\rho\mathbf J$, is

$$
\boxed{\boldsymbol\rho_q=\begin{pmatrix}\sigma_0^{-1}&-B/(nq)\\B/(nq)&\sigma_0^{-1}\end{pmatrix},\qquad \sigma_0=\frac{nq^2\tau}{m}.}
$$

Its off-diagonal signs follow from the stated axes and signed $q$. For zero transverse [electric current](../../../electric-current.md), $E_y/J_x=B/(nq)$ is the Hall [electrical resistivity](../../../electrical-resistivity.md); reversing charge reverses it. The single-species longitudinal [electrical resistivity](../../../electrical-resistivity.md) is independent of $B$ in this ideal isotropic model.

**Adding [electrons](../../../electron.md) and [electron holes](../../../electron-hole.md).** Let both species have density $n$ and charges $q=\pm e$, with $e>0$. The stipulated equal zero-field [electrical conductivity](../../../electrical-conductivity.md) means equal positive [charge carrier mobility](../../../charge-carrier-mobility.md) $\mu=\sigma_0/(ne)$, even if their masses and [momentum relaxation times](../../../momentum-relaxation-time.md) separately differ. Put $r=1/\sigma_0$ and $h=B/(ne)$. Inverting each [electrical resistivity](../../../electrical-resistivity.md) matrix gives

$$
\boldsymbol\sigma_+=\frac1{r^2+h^2}\begin{pmatrix}r&h\\-h&r\end{pmatrix},\qquad \boldsymbol\sigma_-=\frac1{r^2+h^2}\begin{pmatrix}r&-h\\h&r\end{pmatrix}.
$$

Both species experience the same [electric field](../../../electric-field-split.md), so their [electric current](../../../electric-current.md) densities add. Therefore it is their **[conductivity tensors](../../../conductivity-tensor.md)**, rather than their [resistivity tensors](../../../resistivity-tensor.md), that must be summed. The Hall parts cancel and

$$
\boldsymbol\sigma_{\rm tot}=\frac{2\sigma_0}{1+(\mu B)^2}\mathbf I_2,\qquad \boxed{\boldsymbol\rho_{\rm tot}=\frac{1+(\mu B)^2}{2\sigma_0}\mathbf I_2.}
$$

This is [compensated two-carrier magnetoresistance](../../../compensated-two-carrier-magnetoresistance.md). Although the net Hall field vanishes, each carrier species is bent in its own direction; maintaining the total longitudinal [electric current](../../../electric-current.md) requires an increasing longitudinal field. Equal carrier numbers alone do not ensure zero Hall response if [charge carrier mobilities](../../../charge-carrier-mobility.md) differ; both equalities given here are used.

**Large-field limit and quantum oscillations.** Expanding the exact diagonal entry,

$$
\rho_{xx}=\rho_{yy}=\frac1{2\sigma_0}+\frac{\sigma_0B^2}{2n^2e^2}.
$$

For $\mu B\gg1$,

$$
\boxed{\rho_{xx}\sim\rho_{yy}\sim\frac{\sigma_0B^2}{2n^2e^2},\qquad B\gg\frac{ne}{\sigma_0}=\frac{m}{e\tau_{\rm tr}}.}
$$

Here the last equality applies to either species with its own [mass](../../../mass.md) and transport time; the stipulated [charge carrier mobilities](../../../charge-carrier-mobility.md) give the same threshold. This is the classical strong-field condition $\omega_c\tau_{\rm tr}\gg1$: carriers turn substantially before their drift [momentum](../../../momentum-split.md) relaxes.

Observable [quantum oscillations](../../../quantum-oscillation.md) additionally require sufficiently sharp [Landau levels](../../../landau-level.md) and a sufficiently cold [Fermi-Dirac distribution](../../../fermi-dirac-distribution.md), approximately

$$
\omega_c\tau_q\gtrsim1,\qquad \hbar\omega_c\gtrsim k_BT.
$$

When $\tau_q\simeq\tau_{\rm tr}$, the disorder field scale is comparable to the onset scale for large classical [magnetoresistance](../../../magnetoresistance.md). The thermal condition can demand a much larger field, and when $\tau_q\ll\tau_{\rm tr}$ even the disorder criterion is stronger. The quantitative [damping](../../../damping.md) factors in Q2(c) show that these are crossover scales rather than sharp visibility boundaries. A large smooth $B^2$ [magnetoresistance](../../../magnetoresistance.md) therefore does not itself demonstrate [Landau level](../../../landau-level.md); it can exist while thermal smearing suppresses oscillations. Conversely, the asymptotic condition $\omega_c\tau_{\rm tr}\gg1$ is stronger than merely reaching unity, so there is no universal ordering of the two experimental onset fields without temperatures and lifetime information.

**Scaling function.** The material's actual zero-field longitudinal [electrical resistivity](../../../electrical-resistivity.md) is $\rho_{\rm tot}(0)=1/(2\sigma_0)$. Dividing the exact answer by this value gives

$$
\boxed{\frac{\rho_{xx}(B)}{\rho_{xx}(0)}=1+\left(\frac{B\sigma_0}{ne}\right)^2=F(B\sigma_0),\qquad F(x)=1+\frac{x^2}{n^2e^2}.}
$$

The assumption that $n$ stays constant is essential to eliminating further temperature-dependent parameters. $B\sigma_0$ is a dimensionful scaling variable; $B\sigma_0/(ne)=\mu B$ is its dimensionless version. The corresponding fractional increase is $[\rho(B)-\rho(0)]/\rho(0)=(\mu B)^2$.

<a id="4/image-original-equal-mobility-two-carrier-curves-collapse-under-zero-field-resistivity-scaling"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016-compensated-transport.png)

**[Figure 4](#4/image-original-equal-mobility-two-carrier-curves-collapse-under-zero-field-resistivity-scaling). Original equal-mobility two-carrier curves collapse under zero-field resistivity scaling**.

**What the supplied data test.** In the original PDF's left panel, the field dependence is strongly [temperature](../../../temperature-split.md) dependent. In the right panel, plotting the fractional [magnetoresistance](../../../magnetoresistance.md) against the squared rescaled field makes the displayed **125, 150, 175, 200 and 225 K curves collapse approximately onto one straight line**, over the field intervals where they overlap. This supports the proposed one-parameter scaling and, on that range, the quadratic field law. The **100 K curve does not collapse**: it bends away and has a different slope in the rescaled plot. The indicated scaling is therefore supported for the displayed **125–225 K** data, not for the entire displayed [temperature](../../../temperature-split.md) range. The graph alone does not locate a sharp transition between 100 and 125 K or establish behavior above 225 K.

This empirical collapse is [Kohler's rule](../../../kohler-s-rule.md). It is consistent with a common temperature-dependent [charge carrier mobility](../../../charge-carrier-mobility.md) or relaxation scale and a fixed carrier population; it is not a unique proof of exact compensation or of one microscopic scattering mechanism. A change in relative scattering times, carrier population or Fermi-surface structure could spoil the collapse, and this figure alone does not select the cause of the 100 K departure.

There is a factor-of-two normalization convention in the printed text. The $\sigma_0$ introduced for **each** species gives $\rho_{\rm tot}(0)=1/(2\sigma_0)$, whereas the final paragraph calls $1/\sigma_0$ “$\rho_0$.” If $\rho_0$ denotes the experimentally measured zero-field [electrical resistivity](../../../electrical-resistivity.md), the consistent slope is

$$
\frac{\rho(B)-\rho_0}{\rho_0}=\frac1{4n^2e^2}\left(\frac B{\rho_0}\right)^2,\qquad \rho_0=\rho_{\rm tot}(0).
$$

If one instead keeps the literal single-species definition $\rho_s=1/\sigma_0$, the same model has $[\rho(B)-\rho_s]/\rho_s=-1/2+[B/\rho_s]^2/(2n^2e^2)$. The choice rescales and offsets the axes by temperature-independent constants, so it does not change which [temperature](../../../temperature-split.md) curves collapse, but it must be resolved before inferring a [carrier density](../../../carrier-density.md) from the slope.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2016](../../2016-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
