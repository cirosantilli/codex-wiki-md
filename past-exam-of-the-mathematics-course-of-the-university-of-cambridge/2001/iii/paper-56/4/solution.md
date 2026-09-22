<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The basic [parametric surface interrogation](../../../../../parametric-surface-interrogation.md) enquiries provide the parameter domain and patch adjacency; evaluation of $S(u,v)$; first [derivatives](../../../../../derivative.md) $S_u,S_v$; and, for curvature or error-controlled stepping, second [derivatives](../../../../../derivative.md) $S_{uu},S_{uv},S_{vv}$. Useful search enquiries also supply conservative [bounding volumes](../../../../../bounding-volume.md) over parameter rectangles, subdivision or restriction of a patch, and regularity/singularity information. A local inverse or closest-point enquiry can help seed a search but does not replace global component isolation.

At a regular point, $S_u,S_v$ are independent [tangent vectors](../../../../../tangent-vector.md), and the oriented unit [normal vector](../../../../../normal-vector.md) is

$$
\boxed{n=\frac{S_u\times S_v}{|S_u\times S_v|}.}
$$

The [tangent plane](../../../../../tangent-plane.md) consists of $S+\alpha S_u+\beta S_v$. If the cross product is zero, this chart does not define a normal; use a regular alternative chart or treat a true singularity separately.

For two surfaces, collect the four parameters in $w=(u_1,v_1,u_2,v_2)$ and set

$$
F(w)=S_1(u_1,v_1)-S_2(u_2,v_2),\qquad
J=DF=[A_1,-A_2],\qquad A_i=[S_{i,u},S_{i,v}].
$$

At a transverse intersection, $n_1\times n_2\ne0$ and $J$ has rank three. Hence the [implicit function theorem](../../../../../implicit-function-theorem.md) makes $F=0$ locally a curve. Choose its physical unit [tangent vector](../../../../../tangent-vector.md)

$$
\tau=\frac{n_1\times n_2}{|n_1\times n_2|}.
$$

With $G_i=A_i^TA_i$, the parameter derivatives for physical arc length are

$$
\binom{u_i'}{v_i'}=G_i^{-1}A_i^T\tau.
$$

Since $\tau$ lies in both tangent planes, $A_i(u_i',v_i')^T=\tau$ exactly. Thus these two pairs form a vector $d$ in the kernel of $J$.

A practical [transversal intersection of two parametric surfaces](../../../../../transversal-intersection-of-two-parametric-surfaces.md) algorithm is:


- Subdivide parameter patches and reject patch pairs whose certified [bounding volumes](../../../../../bounding-volume.md) are disjoint. Isolate candidate components, including loops wholly inside a patch; edge crossings or a fixed sampling grid alone are not exhaustive. Obtain corrected seeds for all surviving regular components, using a root search on transverse sections where needed.
- At a seed or current point $w$, evaluate points, derivatives and normals, choose the sign of $\tau$ consistently with the preceding step, and predict $w_p=w+\Delta s\,d$ and $X_p=S_1(w)+\Delta s\,\tau$.
- Correct all four parameters by solving the four equations


$$
F(w_c)=0,\qquad \tau\cdot[S_1(u_{1,c},v_{1,c})-X_p]=0
$$

with [Newton method](../../../../../newton-s-method-in-optimization.md). The final equation intersects the curve with the plane through $X_p$ perpendicular to the predicted tangent. Its Jacobian row is $[\tau^TA_1,0,0]$; together with $J$ it is nonsingular at a sufficiently nearby transverse point. This removes the otherwise free along-curve parameter in the three coincidence equations.
- Control $\Delta s$ using correction size, conditioning and curvature/chord error bounds. Reject failed steps and halve the step; keep parameters inside their domains or continue through the declared adjacent patch charts. Store the common corrected point and both parameter pairs.
- Trace both directions until a surface boundary is reached or a previously traced location on the same branch closes the loop. Maintain component/patch records so later seeds do not duplicate an already traced branch, and continue with every remaining seed.

A finite tolerance supplies a polygonal or fitted-curve approximation; regularity and certified bounds determine its accuracy. Parallel normals, singular charts, branch contacts and coincident patches require separate handling: their intersection may be a singular curve, an isolated point or a two-dimensional region. The transverse marching equations must not be used to claim a unique curve in those cases.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
