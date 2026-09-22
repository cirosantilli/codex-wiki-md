<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a scalar fluid property $f(\mathbf x,t)$, the [Eulerian time derivative](../../../../../eulerian-time-derivative.md) $\partial_t f$ measures change at a fixed [Eulerian coordinate](../../../../../eulerian-coordinate.md). The [material derivative](../../../../../material-derivative.md), also called the Lagrangian time derivative, measures change while following one [fluid element](../../../../../fluid-element.md). If its [Lagrangian trajectory](../../../../../lagrangian-trajectory.md) is $\mathbf X(\mathbf a,t)$, where $\mathbf a$ is its fixed [Lagrangian coordinate](../../../../../lagrangian-coordinate.md), then $\partial_t\mathbf X=\mathbf u(\mathbf X,t)$.

The [chain rule](../../../../../chain-rule.md) therefore gives

$$
\boxed{\frac{Df}{Dt}=\frac d{dt}f(\mathbf X(\mathbf a,t),t)=\frac{\partial f}{\partial t}+\mathbf u\cdot\nabla f.}
$$

The last term accounts for entering a region where the property differs. For example, a spatially varying but time-independent [velocity field](../../../../../velocity-field.md) has zero [Eulerian time derivative](../../../../../eulerian-time-derivative.md), while a moving [fluid element](../../../../../fluid-element.md) can have nonzero [material acceleration](../../../../../material-acceleration.md). The same formula applies componentwise to a [vector field](../../../../../vector-field.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
