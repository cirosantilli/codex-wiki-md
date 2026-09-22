<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose the common initial longitude of the particle and $G$ as zero. Let the fixed inertial [longitude of periapsis](../../../../../../longitude-of-periapsis.md) be $\varpi$, positive ahead of that ray. At release $f_0=-\varpi$, but the [mean anomaly](../../../../../../mean-anomaly.md) is

$$
M_0=f_0-2e\sin f_0+O(e^2)=-\varpi+2e\sin\varpi+O(e^2).
$$

Thereafter $M(t)=nt+M_0$, $f(t)=M(t)+2e\sin M(t)+O(e^2)$, and the particle's longitude is $\lambda(t)=\varpi+f(t)$. The reference ray has longitude $\lambda_G=n_gt$.

In the [rotating reference frame](../../../../../../rotating-reference-frame.md), the radial $x$ axis points outward along the star-$G$ ray and the $y$ axis points forward. Define $\delta\lambda=\lambda-\lambda_G$. The exact positional relations are

$$
\boxed{x=r\cos\delta\lambda-a_g,\qquad y=r\sin\delta\lambda.}
$$

<a id="4/iv/image-orbital-angles-and-a-rotating-reference-frame"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-316-rotating-frame.png)

**[Figure 6](#4/iv/image-orbital-angles-and-a-rotating-reference-frame). Orbital angles and a rotating reference frame**. The stellar radius to G defines the rotating radial axis; the particle is separated from it by delta lambda. The pericentre direction is fixed in the inertial frame. The mean anomaly advances uniformly, while the true anomaly is measured from pericentre to the particle.

The diagram shows a later instant; initially $\delta\lambda=0$, so $y(0)=0$. Retaining the $O(e)$ correction in $M_0$ is what will preserve that initial condition in the approximate trajectory.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
