<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [associativity of twisted half-smash products](../../../../../../associativity-of-twisted-half-smash-products.md) follows from an actual isomorphism of the complement bundles. First work over compact parameter spaces, so that a common choice of flags can be made. Choose source, intermediate and target stages $V_i,W_i,Z_i$ satisfying

$$
f_x(V_i)\subset W_i,\qquad g_y(W_i)\subset Z_i.
$$

For the two [twisted half-smash products](../../../../../../twisted-half-smash-product.md) and their composite the relevant [vector bundles](../../../../../../vector-bundle.md) have fibers

$$
\xi_x=W_i\ominus f_x(V_i),\qquad\eta_y=Z_i\ominus g_y(W_i),\qquad\zeta_{y,x}=Z_i\ominus g_yf_x(V_i).
$$

Pull the first two bundles back to $Y\times X$. Since $g_y$ is a [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md), the decomposition of $Z_i$ into $g_y(W_i)$ and its [orthogonal complement](../../../../../../orthogonal-complement.md) gives the fiberwise [vector bundle isomorphism](../../../../../../vector-bundle-isomorphism.md)

$$
\boxed{\zeta_{y,x}=\eta_y\oplus g_y(\xi_x).}
$$

Its inverse is given by the two orthogonal projections. The isomorphism varies continuously with $(y,x)$, and the ranks agree:

$$
\dim Z_i-\dim V_i=(\dim Z_i-\dim W_i)+(\dim W_i-\dim V_i).
$$

The [one-point compactification](../../../../../../alexandroff-extension.md) of an external orthogonal direct sum gives the [smash product](../../../../../../smash-product.md) of its [Thom spaces](../../../../../../thom-space.md). Using $g_y$ to identify $g_y(\xi_x)$ with $\xi_x$, the isomorphism therefore gives

$$
\operatorname{Th}(\zeta)\wedge E(V_i)\cong\operatorname{Th}(\eta)\wedge\operatorname{Th}(\xi)\wedge E(V_i).
$$

The left side is a stage of $(Y\times X)\ltimes_hE$ and the right side is the corresponding two-step prespectrum presentation of $Y\ltimes_g(X\ltimes_fE)$.

These stage comparisons commute with structure maps. Indeed, increasing a stage decomposes a suspension vector into its component in $g_yf_x(V_j\ominus V_i)$ and the two residual complement components. In either construction the same source component is pulled back to $V_j\ominus V_i$ and used in the same structure map of $E$; the residual components are left in the same final complement. Iterated orthogonal decomposition gives the same result whether the intermediate complement is separated first or last. They also commute with maps of $E$, since the comparison only rearranges the suspension coordinates.

For clarity about the intervening [spectrification](../../../../../../spectrification.md), maps out of $LP$ into a genuine indexed spectrum $T$ are precisely compatible prespectrum maps $P\to T$. At stage $i$, adjunction from the Thom coordinate identifies such a map with a continuous family

$$
E(V_i)\longrightarrow\Omega^{(\xi_i)_x}T(W_i)\cong T(f_x(V_i)),
$$

where the last identification is the genuine indexed spectrum structure of $T$. Compatibility between stages is exactly compatibility of this family with the source structure maps. Thus maps out of the twisted construction are continuous families of maps over the specified [linear isometries](../../../../../../linear-isometry-of-hilbert-spaces.md). A family of such maps over $g$ out of $X\ltimes_fE$ is, by applying this universal property a second time, exactly a family of maps out of $E$ over $g_yf_x$. This is the same orthogonal-coordinate correspondence just constructed; it respects the identifications imposed by each [spectrification](../../../../../../spectrification.md). Consequently it descends from the prespectrum presentations to the associated spectra. Common cofinal refinements remove any incompatibility between the independently chosen flags.

The printed hypothesis does not require $Y$ to be compact. For an arbitrary compactly generated parameter space $Y$, use the same construction on compact test spaces mapping into $Y$. Each such family admits the common flags above, and the comparisons agree under restriction because their formula is the canonical orthogonal projection. They therefore assemble into the continuous global comparison in the compactly generated point-set construction. Equivalently, the preceding universal-property correspondence is valid for arbitrary $Y$ and does not impose a uniform finite target stage on all of it. Passing to cellular models for the derived construction gives the requested natural isomorphism

$$
\boxed{Y\ltimes_g(X\ltimes_fE)\cong(Y\times X)\ltimes_hE\quad\text{in the stable homotopy category}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
