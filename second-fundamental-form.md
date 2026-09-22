# Second fundamental form

↑ **Parent:** [Differential geometry](differential-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_fundamental_form)

For an [embedded submanifold](differential-geometry.md#embedded-submanifold) $M\subseteq N$ of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the vector-valued second fundamental form is

$$
A(X,Y)=(\overline\nabla_XY)^\perp.
$$

Here $\overline\nabla$ is the ambient [Levi-Civita connection](general-relativity.md#levi-civita-connection) and the superscript denotes projection onto the [normal bundle](algebraic-geometry.md#normal-bundle). For a hypersurface in Euclidean space with unit normal $N$, the scalar form is $II(X,Y)=\langle A(X,Y),N\rangle=\langle-dN(X),Y\rangle$. In a surface parametrization its coefficients are $e=N\cdot X_{uu}$, $f=N\cdot X_{uv}$, and $g=N\cdot X_{vv}$.

**Table of contents**

- [Totally umbilic hypersurface](#totally-umbilic-hypersurface)
  - [Scalar curvature of an umbilic vacuum hypersurface](#scalar-curvature-of-an-umbilic-vacuum-hypersurface)
- [Zero second fundamental form implies planar image](#zero-second-fundamental-form-implies-planar-image)
- [Fundamental forms of an elliptic ring torus](#fundamental-forms-of-an-elliptic-ring-torus)
- [Second fundamental form of a ring torus](#second-fundamental-form-of-a-ring-torus)
  - [Gaussian curvature of a ring torus](#gaussian-curvature-of-a-ring-torus)
- [Gauss–Codazzi equations](#gauss-codazzi-equations)
  - [Gauss–Codazzi equations for a non-null hypersurface](#gauss-codazzi-equations-for-a-non-null-hypersurface)
  - [Gauss formula](#gauss-formula)
  - [Gauss equation](#gauss-equation)
    - [Gauss equation in a curved ambient manifold](#gauss-equation-in-a-curved-ambient-manifold)
      - [Gauss equation for a nonnull hypersurface](#gauss-equation-for-a-nonnull-hypersurface)
      - [Gauss equation with reversed curvature convention](#gauss-equation-with-reversed-curvature-convention)
      - [Curvature comparison for a geodesically ruled surface](#curvature-comparison-for-a-geodesically-ruled-surface)
    - [Sectional curvature](#sectional-curvature)
      - [Ricci curvature](#ricci-curvature)
        - [Bishop-Gromov inequality](#bishop-gromov-inequality)
          - [Bishop volume comparison with a positive-curvature model](#bishop-volume-comparison-with-a-positive-curvature-model)
            - [Spherical rigidity of maximal total volume](#spherical-rigidity-of-maximal-total-volume)
              - [Maximal diameter rigidity from disjoint comparison balls](#maximal-diameter-rigidity-from-disjoint-comparison-balls)
          - [Euclidean rigidity of maximal asymptotic volume ratio](#euclidean-rigidity-of-maximal-asymptotic-volume-ratio)
        - [Normalized Ricci curvature](#normalized-ricci-curvature)
        - [Isotropic Ricci curvature](#isotropic-ricci-curvature)
        - [Einstein manifold](#einstein-manifold)
          - [Einstein metric](#einstein-metric)
          - [Constant Ricci curvature without constant sectional curvature](#constant-ricci-curvature-without-constant-sectional-curvature)
        - [Sectional curvatures from Ricci curvature in dimension three](#sectional-curvatures-from-ricci-curvature-in-dimension-three)
        - [Scalar curvature](#scalar-curvature)
          - [Constant scalar curvature does not imply an Einstein metric](#constant-scalar-curvature-does-not-imply-an-einstein-metric)
        - [Ricci-flat Riemannian manifold](#ricci-flat-riemannian-manifold)
        - [Myers's theorem](#myers-s-theorem)
          - [Complete positively curved paraboloid](#complete-positively-curved-paraboloid)
          - [Finite fundamental group from a uniform positive Ricci bound](#finite-fundamental-group-from-a-uniform-positive-ricci-bound)
          - [Incomplete positively curved strip with infinite diameter](#incomplete-positively-curved-strip-with-infinite-diameter)
        - [Cheeger-Gromoll splitting theorem](#cheeger-gromoll-splitting-theorem)
          - [Ricci-flat obstruction for a closed three-manifold times a line](#ricci-flat-obstruction-for-a-closed-three-manifold-times-a-line)
      - [Flat manifold](#flat-manifold)
        - [Isometry dimension of a compact flat manifold](#isometry-dimension-of-a-compact-flat-manifold)
        - [Bieberbach theorem](#bieberbach-theorem)
        - [Holonomy groups of closed orientable flat three-manifolds](#holonomy-groups-of-closed-orientable-flat-three-manifolds)
          - [Hantzsche-Wendt manifold](#hantzsche-wendt-manifold)
          - [Sixth-turn flat three-manifold](#sixth-turn-flat-three-manifold)
          - [Third-turn flat three-manifold](#third-turn-flat-three-manifold)
          - [Half-turn flat three-manifold](#half-turn-flat-three-manifold)
        - [Quarter-turn flat three-manifold](#quarter-turn-flat-three-manifold)
        - [Flat torus](#flat-torus)
          - [Short-vector cancellation for flat tori](#short-vector-cancellation-for-flat-tori)
          - [Spectrum of a flat torus](#spectrum-of-a-flat-torus)
            - [Two-dimensional lattice reconstruction from vector lengths](#two-dimensional-lattice-reconstruction-from-vector-lengths)
      - [Cartan-Hadamard theorem](#cartan-hadamard-theorem)
      - [Curvature of the round unit sphere](#curvature-of-the-round-unit-sphere)
  - [Codazzi equation](#codazzi-equation)
- [Tangential derivative of a normal field](#tangential-derivative-of-a-normal-field)
- [Totally geodesic submanifold](#totally-geodesic-submanifold)
  - [An isometry fixed set is totally geodesic](#an-isometry-fixed-set-is-totally-geodesic)
- [Normal curvature](#normal-curvature)
  - [Euler formula for normal curvature](#euler-formula-for-normal-curvature)
    - [Equally spaced normal curvatures average to mean curvature](#equally-spaced-normal-curvatures-average-to-mean-curvature)
- [Symmetry of the second fundamental form](#symmetry-of-the-second-fundamental-form)
- [Shape operator](#shape-operator)
  - [Shape operator in a normal direction](#shape-operator-in-a-normal-direction)
    - [Weingarten formula](#weingarten-formula)
  - [Principal curvature](#principal-curvature)
    - [Principal direction](#principal-direction)
    - [Umbilical point](#umbilical-point)
  - [Euclidean invariance of the shape operator](#euclidean-invariance-of-the-shape-operator)
- [Gaussian curvature](#gaussian-curvature)
  - [Supporting sphere](#supporting-sphere)
    - [Supporting-sphere curvature bound](#supporting-sphere-curvature-bound)
      - [Elliptic point](#elliptic-point)
  - [Gaussian curvature of a cone away from its vertex](#gaussian-curvature-of-a-cone-away-from-its-vertex)
- [Mean curvature](#mean-curvature)
  - [Minimal surface](#minimal-surface)
    - [Coercive-height intersection lemma for a minimal surface](#coercive-height-intersection-lemma-for-a-minimal-surface)
    - [Outer area-minimizing surface](#outer-area-minimizing-surface)
    - [Enneper surface](#enneper-surface)
    - [First variation of area formula](#first-variation-of-area-formula)
    - [Laplacian of a restricted ambient function](#laplacian-of-a-restricted-ambient-function)
      - [Nonexistence of compact Euclidean minimal submanifolds](#nonexistence-of-compact-euclidean-minimal-submanifolds)
  - [Orientation reversal of surface curvature](#orientation-reversal-of-surface-curvature)
- [Fundamental forms of a graph surface](#fundamental-forms-of-a-graph-surface)
  - [Gaussian curvature of a graph surface](#gaussian-curvature-of-a-graph-surface)
  - [Mean-curvature comparison at tangential contact](#mean-curvature-comparison-at-tangential-contact)
    - [Gaussian curvature has no tangential-contact comparison principle](#gaussian-curvature-has-no-tangential-contact-comparison-principle)
  - [Tangency to a plane along a curve forces zero Gaussian curvature](#tangency-to-a-plane-along-a-curve-forces-zero-gaussian-curvature)
  - [Minimal surface equation for a graph](#minimal-surface-equation-for-a-graph)
    - [Bernstein theorem for minimal graphs](#bernstein-theorem-for-minimal-graphs)
    - [Ellipticity of the minimal surface flux](#ellipticity-of-the-minimal-surface-flux)
    - [Gradient maximum principle for a minimal graph](#gradient-maximum-principle-for-a-minimal-graph)
      - [Minimal graphical cone is a plane](#minimal-graphical-cone-is-a-plane)

## Totally umbilic hypersurface

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

At every point its second fundamental form is a scalar multiple of its induced metric. Equivalently its shape operator is scalar, so all principal normal curvatures agree. For a three-dimensional hypersurface, $K=3\lambda$ and $K_{ab}K^{ab}=3\lambda^2$. The sign of its intrinsic scalar in a vacuum Lorentzian ambient space then follows from the [Gauss equation for a nonnull hypersurface](#gauss-equation-for-a-nonnull-hypersurface).

### Scalar curvature of an umbilic vacuum hypersurface

↑ **Parent:** [Totally umbilic hypersurface](#totally-umbilic-hypersurface)

For a timelike unit normal with squared norm epsilon and vanishing ambient Ricci tensor, contraction of the [Gauss equation for a nonnull hypersurface](#gauss-equation-for-a-nonnull-hypersurface) gives the displayed formula. In signature $(+---)$ the timelike normal has epsilon plus one, so the scalar of the induced negative-definite metric is nonnegative. In signature $(-+++)$ the positive-definite spatial metric instead has scalar $-6\lambda^2$. Replacing the induced metric by its negative reverses the scalar, so the inequality must not be transferred between these conventions without adjustment.

// Target: general-relativity.bigb

## Zero second fundamental form implies planar image

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

Differentiate the orthogonality of the unit normal to the two independent coordinate tangent vectors. If the [second fundamental form](second-fundamental-form.md) vanishes, each derivative of the normal is orthogonal to both tangent vectors; differentiating its unit length also makes it orthogonal to the normal. Thus both normal derivatives vanish. On a connected parameter domain the normal is constant, and differentiating the position's scalar product with that constant normal proves the surface lies in a plane.

## Fundamental forms of an elliptic ring torus

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

Rotate an ellipse with positive semiaxes $a,b$ about an axis a distance $r>a$ from its centre. For the [parametrized surface](calculus.md#parametrized-surface) $\sigma(u,v)=((r+a\sin u)\cos v,(r+a\sin u)\sin v,b\cos u)$, put $R=r+a\sin u$ and $D^2=a^2\cos^2u+b^2\sin^2u$. An outward [unit normal](differential-geometry.md#unit-normal) is $N=(b\sin u\cos v,b\sin u\sin v,a\cos u)/D$. Direct [differentiation](calculus.md#differentiation) gives the [first fundamental form](differential-geometry.md#first-fundamental-form) and [second fundamental form](second-fundamental-form.md), with the convention $II_{ij}=\langle\sigma_{ij},N\rangle$:

$$
I=D^2du^2+R^2dv^2,\qquad II=-\frac{ab}{D}du^2-\frac{bR\sin u}{D}dv^2.
$$

Reversing the [unit normal](differential-geometry.md#unit-normal) reverses $II$, but the [Gaussian curvature](#gaussian-curvature) $K=ab^2\sin u/(RD^4)$ is unchanged.

## Second fundamental form of a ring torus

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

For major radius $a>b>0$ and minor radius $b$, let $R=a+b\cos u$. With the inward normal determined by the usual ordered $(u,v)$ parametrization, the [first fundamental form](differential-geometry.md#first-fundamental-form) and [second fundamental form](second-fundamental-form.md) are

$$
I=b^2du^2+R^2dv^2,\qquad II=bdu^2+R\cos u\,dv^2.
$$

Reversing the normal reverses $II$. The [Gaussian curvature of a ring torus](#gaussian-curvature-of-a-ring-torus) is independent of this orientation.

### Gaussian curvature of a ring torus

↑ **Parent:** [Second fundamental form of a ring torus](#second-fundamental-form-of-a-ring-torus)

For a ring [torus](topology.md#torus) of radii $a>b>0$, the [Gaussian curvature](#gaussian-curvature) is

$$
K=\frac{\cos u}{b(a+b\cos u)}.
$$

It is positive on the outer side, negative on the inner side and zero on the top and bottom circles. The sign contrast expresses two principal curvatures of the same sign outside and opposite signs inside.

<h2 id="gauss-codazzi-equations">Gauss–Codazzi equations</h2>

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Codazzi_equations)

The Gauss–Codazzi equations relate the intrinsic curvature and connection of an [embedded submanifold](differential-geometry.md#embedded-submanifold) to its [second fundamental form](second-fundamental-form.md) and the ambient curvature. The [Gauss equation](#gauss-equation) controls tangential curvature; the [Codazzi equation](#codazzi-equation) controls the covariant derivative of the [second fundamental form](second-fundamental-form.md). The [Gauss formula](#gauss-formula) is the tangential-normal splitting used to derive these relations.

<h3 id="gauss-codazzi-equations-for-a-non-null-hypersurface">Gauss–Codazzi equations for a non-null hypersurface</h3>

↑ **Parent:** [Gauss–Codazzi equations](#gauss-codazzi-equations)

For a [hypersurface](differential-geometry.md#hypersurface) with unit [normal vector](differential-geometry.md#normal-vector) $n$, put $\varepsilon=g(n,n)=\pm1$, $P=1-\varepsilon n\otimes n^\flat$, and $K(X,Y)=g(\nabla_Xn,Y)$ for tangent vectors. The [induced metric](riemannian-geometry.md#induced-metric) is nondegenerate precisely when the normal is non-null. With $R(X,Y)Z=[\nabla_X,\nabla_Y]Z-\nabla_{[X,Y]}Z$ and $R_{abcd}=g(e_a,R(e_c,e_d)e_b)$, the [Gauss formula](#gauss-formula) is $\nabla_XY=D_XY-\varepsilon K(X,Y)n$. Substituting twice into the ambient [Riemann curvature tensor](general-relativity.md#riemann-curvature-tensor) and projecting tangentially gives the displayed [Gauss equation](#gauss-equation). Its normal projection gives $g(n,R(X,Y)Z)=-(D_XK)(Y,Z)+(D_YK)(X,Z)$, the curved-ambient [Codazzi equation](#codazzi-equation). A null hypersurface needs additional geometric data because its induced metric is degenerate.

### Gauss formula

↑ **Parent:** [Gauss–Codazzi equations](#gauss-codazzi-equations)

For a submanifold with induced [Levi-Civita connection](general-relativity.md#levi-civita-connection) $\nabla$ and [second fundamental form](second-fundamental-form.md) $A$, the ambient derivative decomposes as

$$
\overline\nabla_XY=\nabla_XY+A(X,Y).
$$

For a parametrized surface this reads $X_{ij}=\Gamma^k_{ij}X_k+h_{ij}N$.

### Gauss equation

↑ **Parent:** [Gauss–Codazzi equations](#gauss-codazzi-equations)

For a Euclidean embedded submanifold,

$$
\langle R(X,Y)Z,W\rangle
=\langle A(X,W),A(Y,Z)\rangle-\langle A(X,Z),A(Y,W)\rangle.
$$

It expresses intrinsic curvature in terms of the [second fundamental form](second-fundamental-form.md).

#### Gauss equation in a curved ambient manifold

↑ **Parent:** [Gauss equation](#gauss-equation)

For an [embedded submanifold](differential-geometry.md#embedded-submanifold) of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), use $R(v,w)y=\nabla_v\nabla_wy-\nabla_w\nabla_vy-\nabla_{[v,w]}y$. The [Gauss formula](#gauss-formula) and [tangential derivative of a normal field](#tangential-derivative-of-a-normal-field) give

$$
\langle\nabla_v\nabla_wy,x\rangle
=\langle D_vD_wy,x\rangle-\langle II(w,y),II(v,x)\rangle.
$$

Subtract the expression with $v,w$ interchanged and the bracket derivative, whose normal part pairs to zero. This proves the displayed curvature identity. For flat Euclidean ambient space, its ambient curvature term vanishes and one obtains the ordinary [Gauss equation](#gauss-equation). Declaring the four-slot convention $R(x,y,v,w)=\langle R(v,w)y,x\rangle$ avoids sign ambiguities when permuting arguments.

##### Gauss equation for a nonnull hypersurface

↑ **Parent:** [Gauss equation in a curved ambient manifold](#gauss-equation-in-a-curved-ambient-manifold)

Let the unit normal satisfy $n^an_a=\varepsilon=\pm1$, let $h_{ab}=g_{ab}-\varepsilon n_an_b$, and set $K_{ab}=h_a{}^ch_b{}^d\nabla_cn_d$. The normal component of an ambient derivative of tangent fields is $-\varepsilon K(X,Y)n$. Substitute that decomposition into the curvature commutator and project tangentially to obtain the displayed equation. Its scalar contraction is ${}^\Sigma R=R-2\varepsilon R_{ab}n^an^b+\varepsilon(K^2-K_{ab}K^{ab})$. Both metric signature and curvature-slot convention must be specified when assigning a sign.

##### Gauss equation with reversed curvature convention

↑ **Parent:** [Gauss equation in a curved ambient manifold](#gauss-equation-in-a-curved-ambient-manifold)

Here $R(X,Y)=D_{[X,Y]}-[D_X,D_Y]$, the negative of the convention in the ordinary [Gauss equation in a curved ambient manifold](#gauss-equation-in-a-curved-ambient-manifold). Insert the [Gauss formula](#gauss-formula) and [Weingarten formula](#weingarten-formula) into this definition and project tangentially to obtain the displayed identity. Positive [sectional curvature](#sectional-curvature) uses $\langle R(X,Y)X,Y\rangle/|X\wedge Y|^2$ with this convention. Thus a Euclidean surface still has [Gaussian curvature](#gaussian-curvature) $K=\det A_\xi$; reversing the operator sign without changing the slot order would give the wrong sign.

##### Curvature comparison for a geodesically ruled surface

↑ **Parent:** [Gauss equation in a curved ambient manifold](#gauss-equation-in-a-curved-ambient-manifold)

A surface locally swept out by ambient [geodesics](riemannian-geometry.md#geodesic) has $II(T,T)=0$ in its unit ruling direction $T$. For a perpendicular unit tangent $E$, the [Gauss equation in a curved ambient manifold](#gauss-equation-in-a-curved-ambient-manifold) therefore gives the displayed identity. Its [Gaussian curvature](#gaussian-curvature) is at most the ambient [sectional curvature](#sectional-curvature) in its tangent plane, with equality precisely when $II(T,E)=0$. An independent variation argument applies the [Jacobi field](general-relativity.md#jacobi-field) equation to the length of a perpendicular connecting field; its ambient derivative has the extra normal component $II(T,E)$. The Euclidean surface $(t,s,ts)$ is ruled by straight lines and has [Gaussian curvature](#gaussian-curvature) $-(1+t^2+s^2)^{-2}<0$.

#### Sectional curvature

↑ **Parent:** [Gauss equation](#gauss-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sectional_curvature)

For a two-plane $\sigma=\operatorname{span}(X,Y)$ in a Riemannian tangent space,

$$
K(\sigma)=\frac{\langle R(X,Y)Y,X\rangle}{|X|^2|Y|^2-\langle X,Y\rangle^2}.
$$

##### Ricci curvature

↑ **Parent:** [Sectional curvature](#sectional-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ricci_curvature)

Ricci curvature is the trace of the Riemann curvature tensor in its first and third arguments. For a unit tangent vector $X$ and an orthonormal basis $X,e_2,\ldots,e_n$,

$$
\operatorname{Ric}(X,X)=\sum_{i=2}^n K(X,e_i).
$$

###### Bishop-Gromov inequality

↑ **Parent:** [Ricci curvature](#ricci-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bishop–Gromov_inequality)

For a complete connected $n$-dimensional [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) with nonnegative [Ricci curvature](#ricci-curvature), the displayed ratio is nonincreasing, tends to one at zero, and is at most one. In particular $\operatorname{Vol}B(p,r)\leq\omega_nr^n$. In [geodesic polar coordinates](riemannian-geometry.md#geodesic-polar-coordinates), the radial [Jacobi field](general-relativity.md#jacobi-field) determinant is at most the Euclidean density $r^{n-1}$ until the cut time. The trace of the [radial Riccati equation for distance spheres](riemannian-geometry.md#radial-riccati-equation-for-distance-spheres), with [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), proves this comparison. Equality for every radius forces the Euclidean polar metric and absence of a [cut locus](riemannian-geometry.md#cut-locus).

###### Bishop volume comparison with a positive-curvature model

↑ **Parent:** [Bishop-Gromov inequality](#bishop-gromov-inequality)

For a complete connected $n$-dimensional [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) with $\operatorname{Ric}\geq(n-1)kg$, $k>0$, put $D=\pi/\sqrt k$ and

$$
s_k(t)=\frac{\sin(\sqrt k\,t)}{\sqrt k},\qquad v_k(r)=\omega_{n-1}\int_0^r s_k(t)^{n-1}\,dt.
$$

Here $\omega_{n-1}$ is the area of the unit $(n-1)$-sphere, and $v_k(r)$ is the [Riemannian volume](differential-geometry.md#riemannian-volume) of a radius-$r$ ball in the round curvature-$k$ [sphere](geometry-and-topology.md#sphere). The [Bishop-Gromov inequality](#bishop-gromov-inequality) asserts that $V_p(r)/v_k(r)$ is nonincreasing for $0<r<D$, tends to one at zero, and is at most one. In [geodesic polar coordinates](riemannian-geometry.md#geodesic-polar-coordinates), the radial volume density before the cut time is at most $s_k(t)^{n-1}$. The bound uses trace [Ricci curvature](#ricci-curvature); with [normalized Ricci curvature](#normalized-ricci-curvature) it reads $\overline{\operatorname{Ric}}\geq kg$.

###### Spherical rigidity of maximal total volume

↑ **Parent:** [Bishop volume comparison with a positive-curvature model](#bishop-volume-comparison-with-a-positive-curvature-model)

Under the hypotheses of [Bishop volume comparison with a positive-curvature model](#bishop-volume-comparison-with-a-positive-curvature-model), the [Bonnet-Myers theorem](#myers-s-theorem) gives diameter at most $D$. If total [Riemannian volume](differential-geometry.md#riemannian-volume) equals $v_k(D)$, every comparison ball ratio is one. In a small normal ball the pointwise radial density bound therefore becomes equality. Writing $h=\partial_r\log J$, the traced [radial Riccati equation for distance spheres](riemannian-geometry.md#radial-riccati-equation-for-distance-spheres) and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) force the radial operator to equal $(s_k'/s_k)I$. The angular metric is consequently $s_k(r)^2g_{S^{n-1}}$, so the metric is locally round. The [classification of complete positive constant-curvature manifolds](riemannian-geometry.md#classification-of-complete-positive-constant-curvature-manifolds) gives a quotient $S_k^n/\Gamma$, whose volume is $v_k(D)/|\Gamma|$. Equality forces $\Gamma$ trivial.

###### Maximal diameter rigidity from disjoint comparison balls

↑ **Parent:** [Spherical rigidity of maximal total volume](#spherical-rigidity-of-maximal-total-volume)

Assume the trace [Ricci curvature](#ricci-curvature) satisfies $\operatorname{Ric}\geq(n-1)kg$, with $k>0$. If points $p,q$ have [Riemannian distance](riemannian-geometry.md#riemannian-distance) $D=\pi/\sqrt k$, the balls $B(p,r)$ and $B(q,D-r)$ are disjoint. [Bishop volume comparison with a positive-curvature model](#bishop-volume-comparison-with-a-positive-curvature-model) bounds their volumes below by $\operatorname{Vol}(M)v_k(r)/v_k(D)$ and $\operatorname{Vol}(M)v_k(D-r)/v_k(D)$. Since $v_k(r)+v_k(D-r)=v_k(D)$, both inequalities must be equalities. Taking $r\downarrow0$ gives $\operatorname{Vol}M=v_k(D)$, and [spherical rigidity of maximal total volume](#spherical-rigidity-of-maximal-total-volume) yields the round sphere.

###### Euclidean rigidity of maximal asymptotic volume ratio

↑ **Parent:** [Bishop-Gromov inequality](#bishop-gromov-inequality)

The [Bishop-Gromov inequality](#bishop-gromov-inequality) forces every volume ratio to equal one if the asymptotic ratio is one. Equality in the radial Jacobian comparison forces the radial operator $A(X)=\nabla_X\partial_r$ of each distance sphere to be $r^{-1}I$ (it is the negative of the outward [shape operator](#shape-operator) in the convention $S=-\nabla\nu$), by the traced [radial Riccati equation for distance spheres](riemannian-geometry.md#radial-riccati-equation-for-distance-spheres) and equality in [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Any finite cut time would remove a positive cone of radial volume at a later radius, contradicting equality. Thus the [Riemannian exponential map](riemannian-geometry.md#exponential-map-riemannian-geometry) is global and one-to-one, and the polar metric is $dr^2+r^2g_{S^{n-1}}$, the Euclidean metric.

###### Normalized Ricci curvature

↑ **Parent:** [Ricci curvature](#ricci-curvature)

For a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension $n\geq2$, the normalized directional [Ricci curvature](#ricci-curvature) averages, rather than sums, the $n-1$ [sectional curvatures](#sectional-curvature) through a unit vector. Thus the [Bonnet-Myers theorem](#myers-s-theorem) gives $\operatorname{diam}M\leq\pi/\sqrt k$ from $\overline{\operatorname{Ric}}\geq kg$. With trace Ricci curvature the corresponding hypothesis is $\operatorname{Ric}\geq(n-1)kg$. The distinction changes positive constants but not the signs of Ricci curvature.

###### Isotropic Ricci curvature

↑ **Parent:** [Ricci curvature](#ricci-curvature)

At a point of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), Ricci curvature is isotropic when $\operatorname{Ric}(v,v)/g(v,v)$ is independent of nonzero tangent direction. Polarization makes this equivalent to the displayed tensor identity. In dimension three, [sectional curvatures from Ricci curvature in dimension three](#sectional-curvatures-from-ricci-curvature-in-dimension-three) gives every sectional curvature at that point the value $c_p/2$. In higher dimensions isotropic Ricci curvature does not determine every two-plane curvature.

###### Einstein manifold

↑ **Parent:** [Ricci curvature](#ricci-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein_manifold)

An [Einstein manifold](#einstein-manifold) has [Ricci curvature](#ricci-curvature) equal to a constant multiple of its metric. In the Riemannian setting, the round unit sphere has $\Lambda=n-1$. This condition is weaker than constant [sectional curvature](#sectional-curvature) in higher dimensions. The definition can also be applied to pseudo-Riemannian metrics, but positivity is assumed in the completeness theorems discussed here.

###### Einstein metric

↑ **Parent:** [Einstein manifold](#einstein-manifold)

A Riemannian or [pseudo-Riemannian metric](differential-geometry.md#pseudo-riemannian-metric) is Einstein when its [Ricci tensor](general-relativity.md#ricci-tensor) is a constant scalar multiple of the metric. Constant-sectional-curvature metrics satisfy this condition with $\Lambda=(d-1)k$. The Killing-form metric on a real [semisimple Lie group](lie-theory.md#semisimple-lie-group) is another example, with $\Lambda=-1/4$ for $g=B$ in the curvature convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$.

###### Constant Ricci curvature without constant sectional curvature

↑ **Parent:** [Einstein manifold](#einstein-manifold)

The [product Riemannian metric](differential-geometry.md#product-riemannian-metric) of two round unit spheres has [Ricci curvature](#ricci-curvature) equal to its metric, since the factor Ricci tensors equal their metrics and the product connection splits. Its directional Ricci curvatures are all one. A two-plane tangent to a single sphere has [sectional curvature](#sectional-curvature) one, while a mixed plane has sectional curvature zero. This four-dimensional [Einstein manifold](#einstein-manifold) therefore need not have constant sectional curvature.

###### Sectional curvatures from Ricci curvature in dimension three

↑ **Parent:** [Ricci curvature](#ricci-curvature)

For an orthonormal triple and distinct $i,j,k$, tracing [sectional curvature](#sectional-curvature) gives $\operatorname{Ric}_{ii}=K_{ij}+K_{ik}$. Solving the three equations gives the displayed formula. Equivalently $K_{ij}=\operatorname{Ric}_{ii}+\operatorname{Ric}_{jj}-\operatorname{Scal}/2$. This pointwise assertion does not require the triple to diagonalize the [Ricci curvature](#ricci-curvature).

###### Scalar curvature

↑ **Parent:** [Ricci curvature](#ricci-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_curvature)

Scalar curvature is the complete trace of the Riemann curvature tensor:

$$
\operatorname{Scal}=\sum_{i,j}\langle R(e_i,e_j)e_j,e_i\rangle.
$$

An $n$-manifold of constant sectional curvature $K$ has $\operatorname{Scal}=n(n-1)K$.

###### Constant scalar curvature does not imply an Einstein metric

↑ **Parent:** [Scalar curvature](#scalar-curvature)

The [product Riemannian metric](differential-geometry.md#product-riemannian-metric) of the round unit two-sphere and a circle has [Ricci curvature](#ricci-curvature) equal to $g_{S^2}$ on the sphere directions and zero on the circle direction. Its [scalar curvature](#scalar-curvature) is constantly two, but no single scalar multiple of the whole metric equals that Ricci tensor. In two dimensions the identity $\operatorname{Ric}=\operatorname{Scal}\,g/2$ does make constant scalar curvature equivalent to an [Einstein metric](#einstein-metric).

###### Ricci-flat Riemannian manifold

↑ **Parent:** [Ricci curvature](#ricci-curvature)

This is the positive-definite metric case of a [Ricci-flat manifold](differential-geometry.md#ricci-flat-manifold).

A Ricci-flat Riemannian manifold has identically zero Ricci tensor. Every flat Riemannian manifold is Ricci-flat, while the converse can fail in dimension at least four.

<h6 id="myers-s-theorem">Myers's theorem</h6>

↑ **Parent:** [Ricci curvature](#ricci-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Myers's_theorem)

For a [connected](geometry-and-topology.md#connected-space) [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension $n\geq2$, assume [geodesic completeness](riemannian-geometry.md#geodesic-completeness) and $\operatorname{Ric}\geq(n-1)\kappa g$ for a constant $\kappa>0$. The [Riemannian distance](riemannian-geometry.md#riemannian-distance) then has diameter at most $\pi/\sqrt\kappa$; the manifold is [compact](topology.md#compact-space) and its [fundamental group](algebraic-topology.md#fundamental-group) is finite. The dimension restriction excludes the vacuous one-dimensional Ricci bound.

###### Complete positively curved paraboloid

↑ **Parent:** [Myers's theorem](#myers-s-theorem)

The graph $z=x^2+y^2$ in Euclidean three-space has the displayed induced [Riemannian metric](differential-geometry.md#riemannian-metric) and positive [Gaussian curvature](#gaussian-curvature). It is smooth at its vertex; the polar-coordinate singularity is only a coordinate artifact. The metric dominates the Euclidean plane metric, so [upward stability of Riemannian completeness](riemannian-geometry.md#upward-stability-of-riemannian-completeness) proves completeness. It has infinite diameter. In dimension two [Ricci curvature](#ricci-curvature) equals Gaussian curvature times the metric, so this is a counterexample to compactness under merely pointwise positive Ricci curvature. Its curvature tends to zero at infinity.

###### Finite fundamental group from a uniform positive Ricci bound

↑ **Parent:** [Myers's theorem](#myers-s-theorem)

If a connected complete [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) has $\operatorname{Ric}\ge(n-1)\kappa g$ with $\kappa>0$, its [universal cover](algebraic-topology.md#universal-cover) with the lifted metric is complete and satisfies the same bound. The [Bonnet-Myers theorem](#myers-s-theorem) makes that cover compact. A covering fiber is closed and discrete and hence finite; the number of its elements equals the order of the [fundamental group](algebraic-topology.md#fundamental-group). Applying the diameter theorem only to the base would not prove this conclusion: the positive lower bound must also be used on the cover.

###### Incomplete positively curved strip with infinite diameter

↑ **Parent:** [Myers's theorem](#myers-s-theorem)

This metric pulls back the round spherical metric by $(u,v)\mapsto(\cos u\cos v,\cos u\sin v,\sin u)$. It has unit [Gaussian curvature](#gaussian-curvature) and [Ricci curvature](#ricci-curvature) equal to its metric, yet the meridian reaches a missing boundary in finite time. Every curve between $(0,0)$ and $(0,L)$ has length at least $|L|/\sqrt2$, so its diameter is infinite. It shows that the positive Ricci bound alone does not replace [geodesic completeness](riemannian-geometry.md#geodesic-completeness) in the [Bonnet-Myers theorem](#myers-s-theorem).

###### Cheeger-Gromoll splitting theorem

↑ **Parent:** [Ricci curvature](#ricci-curvature)

This is a Riemannian [splitting theorem](differential-geometry.md#splitting-theorem) whose hypotheses include a globally minimizing geodesic line.

A complete connected Riemannian manifold with nonnegative Ricci curvature that contains a line splits isometrically as $N\times\mathbb R$.

###### Ricci-flat obstruction for a closed three-manifold times a line

↑ **Parent:** [Cheeger-Gromoll splitting theorem](#cheeger-gromoll-splitting-theorem)

If a connected [closed manifold](differential-geometry.md#closed-manifold) $M^3$ has a noncontractible [universal cover](algebraic-topology.md#universal-cover), then $M\times\mathbb R$ has no complete metric making it a [Ricci-flat Riemannian manifold](#ricci-flat-riemannian-manifold). The product has two ends and hence contains a [line in a Riemannian manifold](riemannian-geometry.md#line-in-a-riemannian-manifold) for any complete metric. The [Cheeger-Gromoll splitting theorem](#cheeger-gromoll-splitting-theorem) would split it isometrically as $N^3\times\mathbb R$. Its three-dimensional factor is Ricci-flat and therefore flat by [three-dimensional curvature from the Ricci tensor](general-relativity.md#three-dimensional-curvature-from-the-ricci-tensor). The complete simply connected cover of the product would be Euclidean four-space. But that cover is $\widetilde M\times\mathbb R$, which retracts onto $\widetilde M$, contradicting noncontractibility.

##### Flat manifold

↑ **Parent:** [Sectional curvature](#sectional-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flat_manifold)

A Riemannian manifold is flat when every sectional curvature is zero. A complete simply connected flat $n$-manifold is isometric to Euclidean space $\mathbb R^n$.

###### Isometry dimension of a compact flat manifold

↑ **Parent:** [Flat manifold](#flat-manifold)

On a compact [flat Riemannian manifold](#flat-manifold), the integrated [Bochner identity for Killing vector fields](general-relativity.md#bochner-identity-for-killing-vector-fields) makes every [Killing vector field](general-relativity.md#killing-vector-field) parallel. Parallel vector fields are exactly the fixed vectors of the linear holonomy. Thus the six orientable closed flat three-manifold types have identity-component isometry dimensions three for the torus, one for each cyclic nontrivial holonomy, and zero for the [Hantzsche-Wendt manifold](#hantzsche-wendt-manifold).

###### Bieberbach theorem

↑ **Parent:** [Flat manifold](#flat-manifold)

The theorem classifies compact [flat manifolds](#flat-manifold) through their crystallographic covering groups.

For a compact [flat Riemannian manifold](#flat-manifold) $\mathbb R^n/\Gamma$, the translations in $\Gamma$ form a normal full-rank [Euclidean lattice](fourier-analysis.md#euclidean-lattice) of finite index. The quotient is its finite linear holonomy. Affine conjugacy of the torsion-free crystallographic groups classifies these manifolds up to affine diffeomorphism. An abelian $\Gamma$ must consist entirely of translations: commuting with every lattice translation forces each linear part to fix a spanning set of $\mathbb R^n$.

###### Holonomy groups of closed orientable flat three-manifolds

↑ **Parent:** [Flat manifold](#flat-manifold)

These are precisely the faithful linear holonomy groups of closed orientable Euclidean three-manifolds. Cyclic cases arise from planar lattice rotations combined with axial screw translations. The noncyclic case is generated by two perpendicular half-turn screws. The list refers to the maximal translation lattice, not to arbitrary finite quotients of a [fundamental group](algebraic-topology.md#fundamental-group).

###### Hantzsche-Wendt manifold

↑ **Parent:** [Holonomy groups of closed orientable flat three-manifolds](#holonomy-groups-of-closed-orientable-flat-three-manifolds)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hantzsche–Wendt_manifold)

The closed orientable [flat Riemannian manifold](#flat-manifold) with holonomy $C_2\times C_2$ can be presented by Euclidean screws $\alpha(x,y,z)=(x+1/2,-y,-z)$ and $\beta(x,y,z)=(-x,y+1/2,-z+1/2)$. Their squares and the square of their product generate the unit translation lattice. Each nonidentity holonomy coset has a half-integer displacement along its fixed axis, so acts freely. The holonomy has no common fixed vector, giving first [Betti number](homology.md#betti-number) zero and a finite [isometry group](riemannian-geometry.md#isometry-group) for every flat metric.

###### Sixth-turn flat three-manifold

↑ **Parent:** [Holonomy groups of closed orientable flat three-manifolds](#holonomy-groups-of-closed-orientable-flat-three-manifolds)

The [mapping torus](algebraic-topology.md#mapping-torus) of an order-six rotation of a hexagonal [flat torus](#flat-torus) is a closed orientable [flat Riemannian manifold](#flat-manifold) with holonomy $C_6$. The screw rotation has angle $\pi/3$ and axial displacement $1/6$. Its first [Betti number](homology.md#betti-number) is one.

###### Third-turn flat three-manifold

↑ **Parent:** [Holonomy groups of closed orientable flat three-manifolds](#holonomy-groups-of-closed-orientable-flat-three-manifolds)

The [mapping torus](algebraic-topology.md#mapping-torus) of an order-three rotation of a hexagonal [flat torus](#flat-torus) is a closed orientable [flat Riemannian manifold](#flat-manifold) with holonomy $C_3$. A screw rotation through $2\pi/3$ with axial displacement $1/3$, together with the planar lattice, describes its deck group. Its first [Betti number](homology.md#betti-number) is one.

###### Half-turn flat three-manifold

↑ **Parent:** [Holonomy groups of closed orientable flat three-manifolds](#holonomy-groups-of-closed-orientable-flat-three-manifolds)

This closed [flat Riemannian manifold](#flat-manifold) is the [mapping torus](algebraic-topology.md#mapping-torus) of $-I$ on a two-dimensional [flat torus](#flat-torus). Equivalently, take planar lattice translations and the screw $(v,z)\mapsto(-v,z+1/2)$ in Euclidean three-space. Its square is a unit axial translation, its holonomy is $C_2$, and its first [Betti number](homology.md#betti-number) is one.

###### Quarter-turn flat three-manifold

↑ **Parent:** [Flat manifold](#flat-manifold)

The Euclidean transformations $a(x,y,z)=(x+1,y,z)$, $b(x,y,z)=(x,y+1,z)$ and $s(x,y,z)=(-y,x,z+1/4)$ generate a torsion-free cocompact group with $sas^{-1}=b$, $sbs^{-1}=a^{-1}$ and $s^4$ equal to unit translation along $z$. Every nontranslation has nonzero axial displacement modulo integers, hence no fixed point. Its maximal translation subgroup is $\mathbb Z^3$ and its holonomy is $C_4$.

###### Flat torus

↑ **Parent:** [Flat manifold](#flat-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flat_torus)

A flat torus is $\mathbb R^d/\Lambda$ with its quotient [Euclidean metric](differential-geometry.md#euclidean-metric), where $\Lambda$ is a full-rank [Euclidean lattice](fourier-analysis.md#euclidean-lattice). Its volume is the lattice covolume. The [dual lattice](fourier-analysis.md#dual-lattice) indexes its complete [Fourier series](fourier-series.md) of [Laplacian eigenfunctions](partial-differential-equation.md#laplacian-eigenfunction).

###### Short-vector cancellation for flat tori

↑ **Parent:** [Flat torus](#flat-torus)

Let $\Lambda_1,\Lambda_2\subset\mathbb R^d$ be full-rank [Euclidean lattices](fourier-analysis.md#euclidean-lattice), and choose $\varepsilon$ smaller than every nonzero vector length in either. The shortest vectors of $\Lambda_i\oplus\varepsilon\mathbb Z^k$ are exactly the new coordinate vectors and their negatives. Any [isometry](riemannian-geometry.md#isometry) between the associated [flat tori](#flat-torus) lifts to an affine [Euclidean isometry](riemannian-geometry.md#euclidean-isometry), whose orthogonal part maps the lattices. It must preserve the span of the shortest vectors, hence also its orthogonal complement, and therefore maps $\Lambda_1$ to $\Lambda_2$. Consequently a nonisometric pair remains nonisometric after adding sufficiently short equal circle factors. The [spectrum of a flat torus](#spectrum-of-a-flat-torus) shows that adding the same factors preserves [isospectral manifolds](riemannian-geometry.md#isospectral-manifolds).

###### Spectrum of a flat torus

↑ **Parent:** [Flat torus](#flat-torus)

With the nonnegative [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator), a frequency $w$ in the [dual lattice](fourier-analysis.md#dual-lattice) gives the [eigenfunction](linear-operator-theory.md#eigenfunction) $e^{2\pi i\langle w,x\rangle}$ and [eigenvalue](linear-operator-theory.md#eigenvalue) $4\pi^2|w|^2$. Its multiplicity is the number of dual vectors with that norm. [Fourier series](fourier-series.md) prove completeness. In dimension two the shortest vector, shortest independent vector and covolume determine a reduced [Gram matrix](linear-algebra.md#gram-matrix), proving [spectral rigidity](riemannian-geometry.md#spectral-rigidity).

###### Two-dimensional lattice reconstruction from vector lengths

↑ **Parent:** [Spectrum of a flat torus](#spectrum-of-a-flat-torus)

The vector-length multiset of a rank-two [Euclidean lattice](fourier-analysis.md#euclidean-lattice) determines it up to an orthogonal map. Let $a$ be the shortest nonzero length. Removing two copies of each positive integer multiple of $a$ removes one primitive lattice line; the shortest remaining length $b$ is the shortest independent-vector length. Those two vectors form a lattice [basis](vector-space.md#basis): otherwise a nonzero point in the centred basis parallelogram would be an independent lattice vector of length less than $b$. Lattice-point density determines the [covolume](fourier-analysis.md#covolume) $A$. The basis [Gram matrix](linear-algebra.md#gram-matrix) then has diagonal entries $a^2,b^2$ and absolute off-diagonal entry $\sqrt{a^2b^2-A^2}$. This proves two-dimensional [spectral rigidity](riemannian-geometry.md#spectral-rigidity) for a [flat torus](#flat-torus) through its [dual lattice](fourier-analysis.md#dual-lattice).

##### Cartan-Hadamard theorem

↑ **Parent:** [Sectional curvature](#sectional-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartan–Hadamard_theorem)

On a complete connected Riemannian manifold of nonpositive sectional curvature, the exponential map at every point is a covering map. If the manifold is simply connected, each exponential map is a diffeomorphism from a tangent space onto the manifold.

##### Curvature of the round unit sphere

↑ **Parent:** [Sectional curvature](#sectional-curvature)

With outward normal $N(x)=x$, the unit sphere has $A(X,Y)=-\langle X,Y\rangle N$. The [Gauss equation](#gauss-equation) therefore gives sectional curvature one on every tangent two-plane.

### Codazzi equation

↑ **Parent:** [Gauss–Codazzi equations](#gauss-codazzi-equations)

For a Euclidean embedded submanifold, the covariant derivative of the second fundamental form satisfies

$$
(\nabla_XA)(Y,Z)=(\nabla_YA)(X,Z).
$$

## Tangential derivative of a normal field

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

For the ambient [Levi-Civita connection](general-relativity.md#levi-civita-connection), a normal field $\eta$, and tangent fields $X,Y$, differentiate $\langle\eta,Y\rangle=0$ using metric compatibility. The tangential part of $\nabla_XY$ is orthogonal to $\eta$, giving the displayed identity. It controls how an ambient derivative of a normal vector can develop a tangential component, and is the vector-valued version of the [shape operator](#shape-operator) relation.

## Totally geodesic submanifold

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

For a [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form) induced [metric tensor](general-relativity.md#metric-tensor), a [totally geodesic submanifold](#totally-geodesic-submanifold) has vanishing [second fundamental form](second-fundamental-form.md); equivalently, every ambient [geodesic](riemannian-geometry.md#geodesic) initially tangent to it remains in it. This extends the notion of a [totally geodesic hypersurface](differential-geometry.md#totally-geodesic-hypersurface) to arbitrary codimension.

### An isometry fixed set is totally geodesic

↑ **Parent:** [Totally geodesic submanifold](#totally-geodesic-submanifold)

A smooth [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form) component of the [fixed-point set](riemannian-geometry.md#fixed-point-set) of an [isometry](riemannian-geometry.md#isometry) is a [totally geodesic submanifold](#totally-geodesic-submanifold). If a [geodesic](riemannian-geometry.md#geodesic) starts tangent to the fixed component, its image under the [isometry](riemannian-geometry.md#isometry) has identical position and tangent. Uniqueness of the [geodesic equation](riemannian-geometry.md#geodesic-equation) makes the two [geodesics](riemannian-geometry.md#geodesic) coincide throughout their common domain, so the original [geodesic](riemannian-geometry.md#geodesic) stays in the fixed set.

## Normal curvature

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_curvature)

The normal curvature of an oriented surface in a unit tangent direction $v$ is

$$
k_n(v)=II(v,v).
$$

It equals the normal component of the acceleration of any unit-speed surface curve tangent to $v$.

### Euler formula for normal curvature

↑ **Parent:** [Normal curvature](#normal-curvature)

If a unit tangent makes angle $\theta$ with the first principal direction, the [normal curvature](#normal-curvature) is $\kappa_n=\kappa_1\cos^2\theta+\kappa_2\sin^2\theta$. This follows by diagonalizing the [second fundamental form](second-fundamental-form.md) relative to the [first fundamental form](differential-geometry.md#first-fundamental-form). When the [Gaussian curvature](#gaussian-curvature) is nonnegative, $|\kappa_n|\leq2|H|$.

#### Equally spaced normal curvatures average to mean curvature

↑ **Parent:** [Euler formula for normal curvature](#euler-formula-for-normal-curvature)

For directions spaced in the same rotational sense, [Euler formula for normal curvature](#euler-formula-for-normal-curvature) gives $k_n(\theta)=H+(k_1-k_2)\cos(2\theta)/2$. The sum of the $m$ equally spaced complex exponentials $e^{2i\theta+2\pi ij/m}$ is zero when $m\geq2$, proving the formula. Consecutive unsigned angles alone do not imply this arrangement: they permit directions to double back.

## Symmetry of the second fundamental form

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

The [second fundamental form](second-fundamental-form.md) of an [embedded submanifold](differential-geometry.md#embedded-submanifold) of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) is symmetric. Its ambient [Levi-Civita connection](general-relativity.md#levi-civita-connection) is a [torsion-free connection](fiber-bundle.md#torsion-free-connection), so

$$
II(X,Y)-II(Y,X)=\bigl(\overline\nabla_XY-\overline\nabla_YX-[X,Y]\bigr)^\perp=0.
$$

The [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) tangent to the submanifold is tangent and therefore has zero normal component. This proof applies to a curved ambient manifold as well as Euclidean space.

## Shape operator

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

The shape operator is an extrinsic-curvature construction in the [differential geometry of surfaces](differential-geometry.md#differential-geometry-of-surfaces).

For an [oriented surface](differential-geometry.md#orientation-of-a-surface) with [Gauss map](differential-geometry.md#gauss-map) $N$, the shape operator at $p$ is the self-adjoint linear map

$$
S_p=-dN_p:T_pS\to T_pS.
$$

### Shape operator in a normal direction

↑ **Parent:** [Shape operator](#shape-operator)

For a normal vector $\xi$, this identity defines the corresponding [shape operator](#shape-operator) using the vector-valued [second fundamental form](second-fundamental-form.md). It is self-adjoint because of the [symmetry of the second fundamental form](#symmetry-of-the-second-fundamental-form). Differentiating $\langle\xi,Y\rangle=0$ shows that $A_\xi X=-(D_X\xi)^\top$. In higher codimension there is a different operator for each normal direction.

#### Weingarten formula

↑ **Parent:** [Shape operator in a normal direction](#shape-operator-in-a-normal-direction)

The [Weingarten formula](#weingarten-formula) decomposes the ambient derivative of a normal field into a tangential [shape operator](#shape-operator) term and the [normal connection](fiber-bundle.md#normal-connection). The minus sign corresponds to $\langle A_\xi X,Y\rangle=\langle II(X,Y),\xi\rangle$. For the outward unit normal of a unit [sphere](geometry-and-topology.md#sphere), $A_\xi=-I$ with this convention.

### Principal curvature

↑ **Parent:** [Shape operator](#shape-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_curvature)

The principal curvatures are the two [eigenvalues](linear-operator-theory.md#eigenvalue) $k_1,k_2$ of the [shape operator](#shape-operator). Thus $K=k_1k_2$ and $H=(k_1+k_2)/2$.

#### Principal direction

↑ **Parent:** [Principal curvature](#principal-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_direction)

A principal direction is an [eigenvector](linear-operator-theory.md#eigenvector) of the [shape operator](#shape-operator). The [normal curvature](#normal-curvature) in a unit principal direction is the corresponding [principal curvature](#principal-curvature).

#### Umbilical point

↑ **Parent:** [Principal curvature](#principal-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Umbilical_point)

An umbilical point of a surface is a point where the two [principal curvatures](#principal-curvature) are equal, equivalently where the [shape operator](#shape-operator) is a scalar multiple of the identity.

### Euclidean invariance of the shape operator

↑ **Parent:** [Shape operator](#shape-operator)

For a [proper Euclidean motion of Euclidean three-space](differential-geometry.md#proper-euclidean-motion-of-euclidean-three-space) $E(x)=Ax+b$, transport the [unit normal](differential-geometry.md#unit-normal) by $\widetilde N(E(p))=AN(p)$. The corresponding shape operators are orthogonally conjugate:

$$
\widetilde S_{E(p)}=A S_p A^{-1}.
$$

Their [determinant](linear-algebra.md#determinant) and [trace](linear-algebra.md#matrix-trace), hence [Gaussian curvature](#gaussian-curvature) and [mean curvature](#mean-curvature), are unchanged.

## Gaussian curvature

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_curvature)

Gaussian curvature is the determinant of the shape operator:

$$
K=\frac{eg-f^2}{EG-F^2}.
$$

### Supporting sphere

↑ **Parent:** [Gaussian curvature](#gaussian-curvature)

A supporting sphere for an embedded surface at $p$ is a sphere tangent at $p$ such that the surface lies locally on one side of the sphere. Comparing second fundamental forms at the tangency controls the surface's [normal curvature](#normal-curvature).

#### Supporting-sphere curvature bound

↑ **Parent:** [Supporting sphere](#supporting-sphere)

If a compact regular surface lies in a closed Euclidean ball of radius $R$, maximize distance from the ball's centre. At a maximizing point, comparison of the [second fundamental form](second-fundamental-form.md) with the tangent [supporting sphere](#supporting-sphere) makes both [principal curvatures](#principal-curvature) have magnitude at least $R^{-1}$ and the same sign. The [Gaussian curvature](#gaussian-curvature) there is therefore at least $R^{-2}$.

##### Elliptic point

↑ **Parent:** [Supporting-sphere curvature bound](#supporting-sphere-curvature-bound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_point)

An elliptic point of a surface is a point at which the [Gaussian curvature](#gaussian-curvature) is positive, equivalently where the two [principal curvatures](#principal-curvature) have the same nonzero sign.

### Gaussian curvature of a cone away from its vertex

↑ **Parent:** [Gaussian curvature](#gaussian-curvature)

Every regular cone parametrized by $X(r,t)=r\,c(t)$ has zero Gaussian curvature away from its vertex. Its unit normal is independent of $r$, while

$$
X_{rr}=0,
\qquad
X_{rt}=c'(t)
$$

is tangent, so two coefficients of the [second fundamental form](second-fundamental-form.md) vanish and $\det II=0$.

## Mean curvature

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_curvature)

The mean curvature vector of an $n$-dimensional embedded submanifold is the trace $\mathbf H=\sum_iA(e_i,e_i)$. For a surface in $\mathbb R^3$, the scalar mean curvature is half the trace of the shape operator:

$$
H=\frac{eG-2fF+gE}{2(EG-F^2)}.
$$

### Minimal surface

↑ **Parent:** [Mean curvature](#mean-curvature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimal_surface)

A minimal submanifold has vanishing mean curvature vector. For a surface in $\mathbb R^3$, this says that the scalar [mean curvature](#mean-curvature) is zero, equivalently that its two [principal curvatures](#principal-curvature) sum to zero.

#### Coercive-height intersection lemma for a minimal surface

↑ **Parent:** [Minimal surface](#minimal-surface)

Let a boundaryless [minimal surface](#minimal-surface) be closed in $\mathbb R^3$, and let its distance to a plane tend to infinity along every sequence escaping bounded sets. If it has no planar point, it must meet the plane. Otherwise absolute signed height has a positive attained minimum by properness. Its Hessian there is semidefinite and equals the [second fundamental form](second-fundamental-form.md) up to sign because the plane is tangent. Minimality makes its trace zero, so the entire form vanishes, contradicting the absence of planar points. This argument uses curvature and attained extrema, rather than an unproved contact comparison for [Gaussian curvature](#gaussian-curvature).

#### Outer area-minimizing surface

↑ **Parent:** [Minimal surface](#minimal-surface)

An [outer area-minimizing surface](#outer-area-minimizing-surface) is a closed surface in a Riemannian initial-data slice whose area is no greater than that of any enclosing competitor. This is a variational property, not a consequence of containment alone. It is important when choosing the horizon-area quantity in the [Riemannian Penrose inequality](general-relativity.md#riemannian-penrose-inequality) and when examining an [apparent-horizon area comparison](general-relativity.md#apparent-horizon-area-comparison).

#### Enneper surface

↑ **Parent:** [Minimal surface](#minimal-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enneper_surface)

The [isothermal coordinates](differential-geometry.md#isothermal-coordinates) $(u,v)$ give the [immersion](differential-geometry.md#immersion) $(u-u^3/3+uv^2,v-v^3/3+u^2v,u^2-v^2)$. Its coordinate functions are harmonic and its metric is $(1+u^2+v^2)^2(du^2+dv^2)$, so it is a complete immersed [minimal surface](#minimal-surface) with self-intersections.

#### First variation of area formula

↑ **Parent:** [Minimal surface](#minimal-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_variation_of_area_formula)

With $A(X,Y)=(\overline\nabla_XY)^\perp$ and $\mathbf H=\operatorname{tr}A$, a variation with velocity $V$ satisfies

$$
\left.\frac d{dt}\operatorname{Area}(M_t)\right|_{t=0}
=-\int_M\langle\mathbf H,V\rangle,d\mu
+\int_{\partial M}\langle V,\eta\rangle,d\sigma.
$$

Thus a boundaryless submanifold is stationary for every compactly supported variation exactly when it is minimal.

#### Laplacian of a restricted ambient function

↑ **Parent:** [Minimal surface](#minimal-surface)

If $M\subseteq\mathbb R^{n+m}$ and $f$ is smooth in the ambient space, then

$$
\Delta_M(f|_M)=\operatorname{tr}_{TM}(\overline{\operatorname{Hess}}f)+\langle\overline\nabla f,\mathbf H\rangle.
$$

##### Nonexistence of compact Euclidean minimal submanifolds

↑ **Parent:** [Laplacian of a restricted ambient function](#laplacian-of-a-restricted-ambient-function)

For the squared distance $r^2(x)=|x|^2$, a minimal $n$-submanifold satisfies $\Delta_Mr^2=2n$. On a compact boundaryless manifold, $r^2$ attains a maximum where the Laplacian is nonpositive, a contradiction for $n>0$.

### Orientation reversal of surface curvature

↑ **Parent:** [Mean curvature](#mean-curvature)

Replacing the chosen [unit normal](differential-geometry.md#unit-normal) $N$ by $-N$ replaces the [shape operator](#shape-operator) $S$ by $-S$. On a surface, [Gaussian curvature](#gaussian-curvature) $K=\det S$ is unchanged, while [mean curvature](#mean-curvature) $H=\operatorname{tr}(S)/2$ changes sign.

## Fundamental forms of a graph surface

↑ **Parent:** [Second fundamental form](second-fundamental-form.md)

For $X(x,y)=(x,y,h(x,y))$ and $W=\sqrt{1+h_x^2+h_y^2}$,

$$
I=
\begin{pmatrix}1+h_x^2&h_xh_y\\h_xh_y&1+h_y^2\end{pmatrix},
\qquad
II=\frac1W
\begin{pmatrix}h_{xx}&h_{xy}\\h_{xy}&h_{yy}\end{pmatrix}.
$$

The upward unit normal is $(-h_x,-h_y,1)/W$.

### Gaussian curvature of a graph surface

↑ **Parent:** [Fundamental forms of a graph surface](#fundamental-forms-of-a-graph-surface)

For the graph of $h$,

$$
K=\frac{h_{xx}h_{yy}-h_{xy}^2}{(1+h_x^2+h_y^2)^2}.
$$

### Mean-curvature comparison at tangential contact

↑ **Parent:** [Fundamental forms of a graph surface](#fundamental-forms-of-a-graph-surface)

Suppose two graph surfaces $z=f(x,y)$ and $z=g(x,y)$ are tangent at the origin, are oriented upward, and $g\geq f$ nearby. Then $g-f$ has a local minimum, so its [Hessian matrix](calculus.md#hessian-matrix) is [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix). At the common horizontal tangent plane,

$$
H_g-H_f=\frac12\operatorname{tr}\operatorname{Hess}(g-f)\geq0.
$$

#### Gaussian curvature has no tangential-contact comparison principle

↑ **Parent:** [Mean-curvature comparison at tangential contact](#mean-curvature-comparison-at-tangential-contact)

The same contact does not order [Gaussian curvature](#gaussian-curvature), because determinant is not monotone under addition of a positive-semidefinite matrix when the original Hessian is indefinite or negative definite. For example,

$$
f=-x^2-y^2,
\qquad
g=-\frac{x^2+y^2}{2}
$$

satisfy $g\geq f$ and are tangent at zero, but $K_g(0)=1<4=K_f(0)$.

### Tangency to a plane along a curve forces zero Gaussian curvature

↑ **Parent:** [Fundamental forms of a graph surface](#fundamental-forms-of-a-graph-surface)

After a rigid motion, write the plane as $z=0$ and the surface locally as $z=h(x,y)$. Along the curve of tangency, $h=0$ and $\nabla h=0$. Differentiating $\nabla h(\gamma(s))=0$ shows that the Hessian annihilates the nonzero tangent $\gamma'(s)$, so its determinant and therefore the Gaussian curvature vanish.

### Minimal surface equation for a graph

↑ **Parent:** [Fundamental forms of a graph surface](#fundamental-forms-of-a-graph-surface)

This equation characterizes a [minimal surface](#minimal-surface) presented as a graph.

The graph of $h$ is minimal exactly when

$$
(1+h_y^2)h_{xx}-2h_xh_yh_{xy}+(1+h_x^2)h_{yy}=0.
$$

Equivalently, it is the Euler--Lagrange equation

$$
\operatorname{div}\frac{\nabla h}{\sqrt{1+|\nabla h|^2}}=0
$$

for the area functional $\int\sqrt{1+|\nabla h|^2}$.

#### Bernstein theorem for minimal graphs

↑ **Parent:** [Minimal surface equation for a graph](#minimal-surface-equation-for-a-graph)

Every entire classical minimal graph over $\mathbb R^n$ is affine for $1\leq n\leq7$. The dimension restriction is essential. This theorem applies to the [minimal surface equation for a graph](#minimal-surface-equation-for-a-graph), without assuming a global bound on its gradient.

// Target: analysis.bigb

#### Ellipticity of the minimal surface flux

↑ **Parent:** [Minimal surface equation for a graph](#minimal-surface-equation-for-a-graph)

The flux $F(p)=p/\sqrt{1+|p|^2}$ of the [minimal surface equation for a graph](#minimal-surface-equation-for-a-graph) has a positive definite [symmetric matrix](linear-algebra.md#symmetric-matrix) derivative. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $(1+|p|^2)^{-3/2}$ in the direction of $p$ and $(1+|p|^2)^{-1/2}$ orthogonally; at $p=0$ every [eigenvalue](linear-operator-theory.md#eigenvalue) is one. On $|p|\leq M$ it satisfies

$$
(1+M^2)^{-3/2}|\xi|^2\leq\xi\cdot DF(p)\xi\leq|\xi|^2.
$$

Thus an [averaged linearization of a nonlinear divergence-form equation](partial-differential-equation.md#averaged-linearization-of-a-nonlinear-divergence-form-equation) is uniformly elliptic where the relevant [gradients](calculus.md#gradient) are bounded. Pointwise positivity alone does not supply a uniform bound on an unbounded gradient range.

#### Gradient maximum principle for a minimal graph

↑ **Parent:** [Minimal surface equation for a graph](#minimal-surface-equation-for-a-graph)

For a $C^2$ solution $u$ of the [minimal surface equation for a graph](#minimal-surface-equation-for-a-graph) on the closure of a bounded domain,

$$
\sup_\Omega|Du|=\sup_{\partial\Omega}|Du|.
$$

Write $a^{ij}(Du)u_{ij}=0$ with $a^{ij}(p)=\delta_{ij}-p_ip_j/(1+|p|^2)$. Its differentiated operator $\mathcal L=a^{ij}D_{ij}+b^\ell D_\ell$, where $b^\ell=(\partial a^{ij}/\partial p_\ell)u_{ij}$, satisfies

$$
\mathcal L|Du|^2=2\sum_k a^{ij}u_{ki}u_{kj}\geq0.
$$

The [weak maximum principle for elliptic operators](elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) gives the result. Interior [Schauder estimates](elliptic-boundary-value-problem.md#schauder-estimates) justify differentiating a solution initially assumed only $C^2$.

##### Minimal graphical cone is a plane

↑ **Parent:** [Gradient maximum principle for a minimal graph](#gradient-maximum-principle-for-a-minimal-graph)

If a smooth [minimal surface equation for a graph](#minimal-surface-equation-for-a-graph) solution on $\mathbb R^n\setminus\{0\}$ is homogeneous of degree one, with $n\geq2$, then its graph extends to a plane through zero. Its [gradient](calculus.md#gradient) is homogeneous of degree zero, so $|Du|^2$ attains a global maximum on the unit sphere. The [strong maximum principle for elliptic operators](elliptic-boundary-value-problem.md#strong-maximum-principle-for-elliptic-operators) makes it constant. The differentiated equation in the [gradient maximum principle for a minimal graph](#gradient-maximum-principle-for-a-minimal-graph) then forces $D^2u=0$, and degree-one homogeneity removes the affine constant. This argument applies to cones that are graphs of smooth functions away from their vertex; it is not a claim that every [minimal surface](#minimal-surface) cone is flat.

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (53)

- [Basic-function Laplacian identity](differential-geometry.md#basic-function-laplacian-identity)
- [Coercive-height intersection lemma for a minimal surface](#coercive-height-intersection-lemma-for-a-minimal-surface)
- [Differential geometry of surfaces](differential-geometry.md#differential-geometry-of-surfaces)
- [Euler formula for normal curvature](#euler-formula-for-normal-curvature)
- [Fundamental forms of an elliptic ring torus](#fundamental-forms-of-an-elliptic-ring-torus)
- [Gauss–Codazzi equations](#gauss-codazzi-equations)
- [Gauss equation](#gauss-equation)
- [Gauss formula](#gauss-formula)
- [Gaussian curvature of a cone away from its vertex](#gaussian-curvature-of-a-cone-away-from-its-vertex)
- [Parametric surface interrogation](differential-geometry.md#parametric-surface-interrogation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-74.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-57.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#12a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2.md#12h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3.md#2h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2.md#24h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#23h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3.md#12a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#24h/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3.md#2g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#23h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4.md#12g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#24h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#24h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#24i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-16.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#15f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#14g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#14g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#25i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#25h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-311.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#26f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#26i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3.md#25i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-115.md#1/a/solution)
- [Second fundamental form of a ring torus](#second-fundamental-form-of-a-ring-torus)
- [Shape operator in a normal direction](#shape-operator-in-a-normal-direction)
- [Smooth embedded surface](differential-geometry.md#smooth-embedded-surface)
- [Supporting-sphere curvature bound](#supporting-sphere-curvature-bound)
- [Symmetry of the second fundamental form](#symmetry-of-the-second-fundamental-form)
- [Totally geodesic submanifold](#totally-geodesic-submanifold)
- [Zero second fundamental form implies planar image](#zero-second-fundamental-form-implies-planar-image)
