<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Let $\Theta=\angle AOB$ and let the [sphere](../../../../../sphere.md) have radius $R$. By rotational invariance, condition on $A$ and place it at the north pole. A band at polar angle $\theta$ has [surface area](../../../../../surface-area.md) $2\pi R^2\sin\theta\,d\theta$, while the sphere has area $4\pi R^2$. Thus the [central angle between independent uniform sphere points](../../../../../central-angle-between-independent-uniform-sphere-points.md) has density

$$
\boxed{f_\Theta(\theta)=\frac12\sin\theta\quad(0<\theta<\pi),}
$$

with density zero outside that interval.

Condition now on $A,B$ with their angle fixed at $\theta$. For $\angle AOC$ and $\angle BOC$ to be acute, the unit position [vector](../../../../../vector.md) of $C$ must have positive [dot products](../../../../../dot-product.md) with both unit vectors of $A$ and $B$. Hence $C$ must lie in the intersection of the two corresponding open [hemispheres](../../../../../hemisphere.md). The great circles bounding them meet at the two antipodes perpendicular to the plane of $A,B$. Their common hemisphere region is a [spherical lune](../../../../../spherical-lune.md) of opening $\pi-\theta$: when $A=B$ it is a hemisphere of opening $\pi$, and as the two normals separate, that opening decreases by $\theta$. More explicitly, take the common boundary antipodes as poles. The longitude conditions each allow an interval of length $\pi$, with their centres separated by $\theta$, so the intersection has longitude width $\pi-\theta$.

Integrating the spherical area element $R^2\sin\varphi\,d\varphi\,d\lambda$ over that lune gives area $2R^2(\pi-\theta)$. Thus the conditional probability that the two angles involving $C$ are acute is $(\pi-\theta)/(2\pi)$. The remaining angle $\Theta$ must itself be acute, so the desired probability is

$$
P=\int_0^{\pi/2}\frac{\pi-\theta}{2\pi}\frac{\sin\theta}{2}\,d\theta.
$$

Integration by parts gives $\int_0^{\pi/2}\theta\sin\theta\,d\theta=1$, while $\int_0^{\pi/2}\sin\theta\,d\theta=1$. Therefore

$$
\boxed{P=\frac{\pi-1}{4\pi}.}
$$

This calculates [pairwise acute central angles of three uniform sphere points](../../../../../pairwise-acute-central-angles-of-three-uniform-sphere-points.md) by conditional area, rather than incorrectly treating the three angle events as independent. Boundary right angles have probability zero, so choosing open rather than closed hemispheres does not change the result.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
