# Group velocity in material and vacuum wavelength coordinates

↑ **Parent:** [Group velocity](group-velocity.md)

Writing the material [wavelength](wavelength.md) as $\lambda_m=2\pi/k$ and its [phase velocity](phase-velocity.md) as $v_p(\lambda_m)$ gives $v_g=v_p-\lambda_m\,dv_p/d\lambda_m$. This follows by differentiating $\omega=kv_p$ and using $k\,d\lambda_m/dk=-\lambda_m$. If instead the independent variable is vacuum wavelength $\lambda_0=2\pi c/\omega$, then $k=\omega/v_p(\lambda_0)$ gives

$$
\boxed{v_g=\frac{v_p}{1+(\lambda_0/v_p)\,dv_p/d\lambda_0}
=\frac{c}{n-\lambda_0\,dn/d\lambda_0}}.
$$

Substituting vacuum wavelengths into the material-wavelength derivative formula gives an erroneous result beyond first order in dispersion. The two coordinates describe the same [dispersion relation](dispersion-relation-split.md), but their derivatives differ by the chain rule.

## ↑ Ancestors (9)

1. [Group velocity](group-velocity.md)
2. [Phase velocity and group velocity](phase-velocity-and-group-velocity.md)
3. [Dispersion relation](dispersion-relation-split.md)
4. [Wave equation](wave-equation-split.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Which wavelength enters the derivative formula](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-b/b7/which-wavelength-enters-the-derivative-formula.md)
