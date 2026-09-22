<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

One definition of a [principal bundle](../../../../../principal-bundle.md) $P\to M$ uses local trivializations $\phi_i:\pi^{-1}(U_i)\to U_i\times G$ whose overlap maps are

$$
\phi_j\phi_i^{-1}(x,g)=(x,t_{ji}(x)g),
$$

with smooth $G$-valued [transition functions of a principal bundle](../../../../../transition-function-of-a-principal-bundle.md) satisfying the cocycle condition. This definition displays the global right [group action](../../../../../group-action.md) rather than assuming it: if $\phi_i(p)=(x,g_i)$, define $\phi_i(p\cdot h)=(x,g_i h)$. On an overlap,

$$
t_{ji}(x)(g_i h)=(t_{ji}(x)g_i)h,
$$

so the local definitions agree. The resulting action is smooth, free and transitive on each fibre, and respects the projection.

If $s:M\to P$ is a global [section of a fiber bundle](../../../../../section-fiber-bundle.md), set $F(x,h)=s(x)\cdot h$. The free and transitive fibre action makes $F:M\times G\to P$ bijective. In a local trivialization, write $s(x)=(x,a_i(x))$; then $F(x,h)=(x,a_i(x)h)$ and its inverse is $(x,g)\mapsto(x,a_i(x)^{-1}g)$. Both are smooth and respect the action and projection. Conversely a [principal bundle](../../../../../principal-bundle.md) isomorphism $M\times G\to P$ sends $x\mapsto(x,e)$ to a global section. Hence

$$
\boxed{P\text{ admits a global section}\ \Longleftrightarrow\ P\cong M\times G\text{ as a principal bundle}.}
$$

For a [pseudo-Riemannian manifold](../../../../../pseudo-riemannian-manifold.md) of [metric signature](../../../../../metric-signature.md) $(p,q)$, its [orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md) has fibre at $x$ consisting of linear isometries $u:\mathbb R^{p,q}\to T_xM$. Its structure group is $O(p,q)$ and its right action is $u\cdot h=u\circ h$. Two such frames differ by a unique element of $O(p,q)$, proving the required free and transitive fibre action. A global section is exactly a global [pseudo-orthonormal frame](../../../../../pseudo-orthonormal-frame.md). Orientation and time orientation, when specified, restrict the structure group and the allowed frames.

Realize unit-radius four-dimensional [de Sitter spacetime](../../../../../de-sitter-spacetime.md) as

$$
\mathrm{dS}_4=\{X\in\mathbb R^{4,1}:\eta(X,X)=1\},\qquad \eta=\operatorname{diag}(-1,1,1,1,1).
$$

Its tangent space is $X^\perp$, with Lorentzian [metric signature](../../../../../metric-signature.md) $(3,1)$. If $e_0,e_1,e_2,e_3$ is a [pseudo-orthonormal frame](../../../../../pseudo-orthonormal-frame.md) at $X$, append $X$ as the final column. The resulting five-by-five matrix preserves $\eta$, and conversely every such matrix supplies a point $X$ and a frame at that point. Thus the full frame bundle is $O(4,1)$, with projection $g\mapsto ge_4$ and fibre group $O(3,1)$.

The printed $SO(4,1)$ statement requires the orientation restriction. Choose the tangent orientation by requiring the appended matrix to have determinant one. Then

$$
\boxed{SO(4,1)\longrightarrow\mathrm{dS}_4,\qquad g\longmapsto ge_4,}
$$

is precisely the [oriented frame bundle of de Sitter spacetime](../../../../../oriented-frame-bundle-of-de-sitter-spacetime.md), with right structure group $SO(3,1)$ embedded as $\operatorname{diag}(h,1)$. If future time orientation is also required, use $SO_0(4,1)$ and $SO_0(3,1)$. Calling $SO(4,1)$ the full bundle without specifying orientation would exclude valid frames of the opposite orientation.

Finally write the global coordinates

$$
X(\tau,n)=(\sinh\tau,\cosh\tau\,n),\qquad \tau\in\mathbb R,\quad n\in S^3.
$$

Direct differentiation gives the [de Sitter spacetime](../../../../../de-sitter-spacetime.md) metric $-d\tau^2+\cosh^2\tau\,g_{S^3}$. The assumed global [frame of a vector bundle](../../../../../frame-of-a-vector-bundle.md) on $S^3$ can be orthonormalized smoothly by [Gram-Schmidt orthogonalization](../../../../../gram-schmidt-process.md) for the round positive metric. More explicitly, view $S^3$ as the [unit quaternions](../../../../../unit-quaternion.md): $Y_1(q)=qi$, $Y_2(q)=qj$, $Y_3(q)=qk$ form a smooth global orthonormal tangent basis. Set

$$
E_0=\partial_\tau,\qquad E_i=(\cosh\tau)^{-1}Y_i,\quad i=1,2,3.
$$

These have inner products $g(E_0,E_0)=-1$, $g(E_i,E_j)=\delta_{ij}$ and $g(E_0,E_i)=0$. They are smooth everywhere because $\cosh\tau$ never vanishes. Choose the spatial orientation consistently, reversing one $Y_i$ if necessary, and choose $E_0$ future-directed. This [global frame on four-dimensional de Sitter spacetime](../../../../../global-frame-on-four-dimensional-de-sitter-spacetime.md) yields a global section of the full frame bundle and also of either restricted bundle. **Yes: the de Sitter frame bundle admits a global section and is trivial.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
