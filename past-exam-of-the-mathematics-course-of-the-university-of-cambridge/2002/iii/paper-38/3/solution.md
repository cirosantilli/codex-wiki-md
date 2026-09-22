<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [transformation model](../../../../../transformation-model.md) consists of a [group](../../../../../group-split.md) $G$ acting on the [sample space](../../../../../sample-space.md) and on the set of [statistical parameters](../../../../../statistical-parameter.md), with the compatibility property

$$
P_{g\theta}=g_*P_\theta,\qquad g\in G.
$$

In words, transforming a sample from $P_\theta$ produces a sample from $P_{g\theta}$. A transitive [transformation model](../../../../../transformation-model.md) is generated from one reference distribution by the [group action](../../../../../group-action.md). For densities, the compatibility property includes the [Jacobian determinant](../../../../../jacobian-determinant.md) of the sample transformation; it is not merely equality of [density](../../../../../density.md) values at transformed points.

A [maximal invariant](../../../../../maximal-invariant.md) $A$ is constant on [orbits of a group action](../../../../../orbit-of-a-group-action.md) and separates them: $A(gx)=A(x)$, and $A(x)=A(y)$ implies $y=gx$ for some $g$. An [equivariant estimator](../../../../../equivariant-estimator.md) $T$ of the parameter satisfies $T(gx)=gT(x)$. Equivariance means the estimate follows the transformed parameter, whereas invariance means the reported value stays unchanged.

First suppose the set of [statistical parameters](../../../../../statistical-parameter.md) can be identified with the [group](../../../../../group-split.md), as happens for a simply transitive action. An [equivariant estimator](../../../../../equivariant-estimator.md) then provides a group-valued fit $\widehat g(x)$ with $\widehat g(gx)=g\widehat g(x)$. Normalize the sample by this fit:

$$
\boxed{A(x)=\widehat g(x)^{-1}x.}
$$

Indeed $A(gx)=\widehat g(x)^{-1}g^{-1}gx=A(x)$. Conversely, if $A(x)=A(y)$, then $y=\widehat g(y)\widehat g(x)^{-1}x$, placing $x,y$ in the same [orbit of a group action](../../../../../orbit-of-a-group-action.md). This establishes maximality, rather than only invariance.

For a transitive action with a nontrivial [stabilizer](../../../../../stabilizer-subgroup.md) $H$ of a reference parameter $\theta_0$, a parameter-valued [equivariant estimator](../../../../../equivariant-estimator.md) does not specify a unique normalizing transformation. Choose a section $h_\theta$ with $h_\theta\theta_0=\theta$ and form $b(x)=h_{T(x)}^{-1}x$. Under $g$,

$$
b(gx)=h_{gT(x)}^{-1}g h_{T(x)}b(x),\qquad h_{gT(x)}^{-1}g h_{T(x)}\in H.
$$

Thus the $H$-orbit of $b(x)$ is invariant. It is maximal: if $b(y)=h b(x)$ with $h\in H$, then $y=h_{T(y)}h h_{T(x)}^{-1}x$. Appropriate [measurable](../../../../../measurability.md) sections and [orbit of a group action](../../../../../orbit-of-a-group-action.md) coordinates are assumed when treating this as a [statistic](../../../../../statistic.md). This qualification explains why an arbitrary equivariant [statistic](../../../../../statistic.md) alone is not automatically a complete set of invariant coordinates.

For the [location-scale family](../../../../../location-scale-family.md), write $X_i=\mu+\sigma Z_i$ with $\sigma>0$ and a fixed joint distribution of $Z$. The [group](../../../../../group-split.md) consists of maps $x_i\mapsto a+bx_i$ with $b>0$, acting on parameters by $(\mu,\sigma)\mapsto(a+b\mu,b\sigma)$. For a nonconstant sample of size $n\ge2$, take the [equivariant estimator](../../../../../equivariant-estimator.md)

$$
\widehat\mu=\overline X,\qquad \widehat\sigma=s=\left\{\frac1n\sum_i(X_i-\overline X)^2\right\}^{1/2}.
$$

It gives the [maximal invariant](../../../../../maximal-invariant.md)

$$
\boxed{A(X)=\left(\frac{X_1-\overline X}s,\ldots,\frac{X_n-\overline X}s\right).}
$$

Its coordinates satisfy $\sum_iA_i=0$ and $\sum_iA_i^2=n$. They stay unchanged under location and positive-scale transformations. If two samples have the same standardized [vector](../../../../../vector.md), then

$$
y_i=\overline y+\frac{s_y}{s_x}(x_i-\overline x),
$$

so a single [group](../../../../../group-split.md) transformation maps the first sample onto the second. The [vector](../../../../../vector.md) retains the observation labels: sorting it would discard information not removed by this location-scale [group](../../../../../group-split.md). The construction is algebraic and does not require the underlying distribution to have finite [moments](../../../../../moment.md). Constant samples can be assigned a separate invariant value; they form a single exceptional [orbit of a group action](../../../../../orbit-of-a-group-action.md) and have probability zero under an independent continuous base distribution.

Finally, in a transitive [transformation model](../../../../../transformation-model.md) every invariant [statistic](../../../../../statistic.md) is ancillary. Choose $g$ taking $\theta_0$ to $\theta$ and use $X_\theta\overset d=gX_{\theta_0}$; invariance gives $A(X_\theta)\overset d=A(X_{\theta_0})$. Thus the standardized residual configuration provides a natural conditioning variable, while the equivariant fit contains the location and scale information.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
