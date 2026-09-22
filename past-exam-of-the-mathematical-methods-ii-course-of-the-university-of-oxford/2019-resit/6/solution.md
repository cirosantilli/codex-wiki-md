<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For an oriented piecewise smooth [surface](../../../topological-surface-split.md) $S$, a continuously differentiable [vector field](../../../vector-field.md) $F$ on a neighborhood of it, and its compatibly oriented boundary $C=\partial S$, [Stokes theorem](../../../stokes-theorem.md) states

$$
\boxed{\oint_CF\cdot d r=\iint_S(\nabla\times F)\cdot n\,dS.}
$$

Here $n$ is the chosen unit [normal vector](../../../normal-vector.md), $dS$ is the unsigned [surface area element](../../../surface-area-element.md), and $d r$ is the tangent displacement along $C$. The [right-hand rule](../../../right-hand-rule.md) relates the boundary direction to $n$.

The supplied field has [curl](../../../curl.md) $\nabla\times F=(2z,2x,2y)$. Parametrize the plane by $r(x,y)=(x,y,1-x-y)$ over the triangle $D=\{x,y\geq0:x+y\leq1\}$. Its upward oriented [surface area element](../../../surface-area-element.md) is $(1,1,1)\,dx\,dy$, giving

$$
\iint_S(\nabla\times F)\cdot d\boldsymbol S
=\int_D2(x+y+z)\,dx\,dy
=2\operatorname{area}(D)=\boxed{1}.
$$

For the boundary [line integral](../../../line-integral.md), take the positively oriented vertices $A=(1,0,0)$, $B=(0,1,0)$, $C=(0,0,1)$. Their projections run counterclockwise in the horizontal plane. With $0\leq t\leq1$, the three edges are

$$
r_{AB}=(1-t,t,0),\qquad r_{BC}=(0,1-t,t),\qquad r_{CA}=(t,0,1-t).
$$

On each edge, direct substitution gives $F(r(t))\cdot r'(t)=t^2+2t-1$. Hence

$$
\boxed{\oint_CF\cdot d r
=3\int_0^1(t^2+2t-1)\,dt=3\left(\frac13\right)=1.}
$$

The two independent computations agree, including the orientation sign.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
