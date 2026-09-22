<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) is $df/d\eta=0$. At first order, directional deflections act only on the isotropic background and hence give no angular contribution. Differentiating $f=\bar f-\Theta\,d\bar f/d\ln\epsilon$ along the unperturbed trajectory gives

$$
0=\frac{d\bar f}{d\ln\epsilon}
\left[\frac{d\ln\epsilon}{d\eta}-
(\partial_\eta+\mathbf e\cdot\nabla)\Theta\right].
$$

Using the tensor redshift of the comoving energy,

$$
\boxed{\dot\Theta+\mathbf e\cdot\nabla\Theta
=-\frac12\dot h_{ij}e^ie^j}.
$$

The [method of characteristics](../../../../../../method-of-characteristics.md) follows the backward ray $\mathbf x(\eta')=\mathbf x-(\eta-\eta')\mathbf e$. With zero initial perturbation, the line-of-sight solution is

$$
\boxed{\Theta(\eta,\mathbf x,\mathbf e)
=-\frac12\int_0^\eta d\eta'\,
\dot h_{ij}\bigl(\eta',\mathbf x-(\eta-\eta')\mathbf e\bigr)e^ie^j}.
$$

To this order the frame and coordinate direction components may be identified inside a quantity already proportional to $h$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
