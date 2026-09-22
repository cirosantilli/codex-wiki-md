<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

An [immersion](../../../../../immersion.md) $\phi:U\to\mathbb R^3$ has differential of rank $2$, equivalently [linearly independent](../../../../../linear-independence.md) $\phi_u,\phi_v$. It has [isothermal coordinates](../../../../../isothermal-coordinates.md) when its [first fundamental form](../../../../../first-fundamental-form.md) has $E=G>0$, $F=0$. A [minimal surface](../../../../../minimal-surface.md) has zero [mean curvature](../../../../../mean-curvature.md).

For an isothermal [immersion](../../../../../immersion.md), differentiation of $E=G$ and $F=0$ gives

$$
(\phi_{uu}+\phi_{vv})\cdot\phi_u=\tfrac12E_u+F_v-\tfrac12G_u=0,
$$

and similarly its scalar product with $\phi_v$ is zero. Its normal component is $e+g$. The given [mean curvature](../../../../../mean-curvature.md) formula reduces to $H=(e+g)/(2E)$, so

$$
\boxed{\phi_{uu}+\phi_{vv}=2EH\mathbf n.}
$$

Thus an isothermal [immersion](../../../../../immersion.md) is minimal exactly when each coordinate is a [harmonic function](../../../../../harmonic-function.md).

An explicit example is the [Enneper surface](../../../../../enneper-surface.md), parametrized on $\mathbb R^2$ by

$$
\phi(u,v)=(u-u^3/3+uv^2,\ v-v^3/3+u^2v,\ u^2-v^2).
$$

Every coordinate has zero Laplacian. Direct differentiation gives $\phi_u\cdot\phi_v=0$ and $|\phi_u|^2=|\phi_v|^2=(1+u^2+v^2)^2>0$. Thus it is an isothermal [immersion](../../../../../immersion.md) and is minimal everywhere.

It is not an open subset of any of the three listed surfaces. The parameter points $(\sqrt3,0)$ and $(-\sqrt3,0)$ both map to $(0,0,3)$, but their tangent planes differ: $\phi_u=(-2,0,\pm2\sqrt3)$ while $\phi_v=(0,4,0)$. A plane, [catenoid](../../../../../catenoid.md), or [helicoid](../../../../../helicoid.md) is an embedded smooth surface with a unique tangent plane at each point. If our whole image lay in any one of them, both rank-$2$ tangent planes at this point would have to equal its tangent plane, a contradiction.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
