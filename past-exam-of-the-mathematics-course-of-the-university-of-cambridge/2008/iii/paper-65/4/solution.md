<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The given equation is a [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md), with the sign appropriate to the chosen invariant coframe. Write $\lambda=(\lambda_{ij})$ as an antisymmetric matrix of one-forms, so $d\lambda=\lambda\wedge\lambda$. Using the graded product rule for the [exterior derivative](../../../../../exterior-derivative.md),

$$
\begin{aligned}
d^2\lambda_{ij}
&=d\lambda_{ik}\wedge\lambda_{kj}-\lambda_{ik}\wedge d\lambda_{kj}\\
&=\lambda_{i\ell}\wedge\lambda_{\ell k}\wedge\lambda_{kj}
-\lambda_{ik}\wedge\lambda_{k\ell}\wedge\lambda_{\ell j}=0.
\end{aligned}
$$

The two sums coincide after exchanging their dummy indices $k,\ell$. This is also associativity of matrix-valued [wedge products of differential forms](../../../../../wedge-product-of-differential-forms.md).

To make the relation to the [Jacobi identity](../../../../../jacobi-identity.md) explicit, let $\theta^a$ be any independent coframe and write $d\theta^a=-\frac12c^a{}_{bc}\theta^b\wedge\theta^c$. Its dual invariant vector fields satisfy $[E_b,E_c]=c^a{}_{bc}E_a$, by the [exterior derivative of a one-form evaluated on vector fields](../../../../../exterior-derivative-of-a-one-form-evaluated-on-vector-fields.md). Evaluating $d^2\theta^a=0$ on three basis fields gives the cyclic coefficient identity

$$
c^e{}_{bc}c^a{}_{ed}+c^e{}_{cd}c^a{}_{eb}+c^e{}_{db}c^a{}_{ec}=0.
$$

These are exactly the components of $[[E_b,E_c],E_d]+[[E_c,E_d],E_b]+[[E_d,E_b],E_c]=0$. Thus **the structure constants obey the Jacobi identity**.

For the real four-dimensional case, abbreviate $a=\lambda_{12}$, $b=\lambda_{23}$, $c=\lambda_{31}$, $d=\lambda_{43}$, $e=\lambda_{41}$, $f=\lambda_{42}$; here $d$ without an argument is a one-form, whereas $d(\cdot)$ denotes the [exterior derivative](../../../../../exterior-derivative.md). Directly expanding the given equations gives

$$
\begin{array}{lll}
d a=-b\wedge c-e\wedge f,&d b=-c\wedge a+d\wedge f,&d c=-a\wedge b-d\wedge e,\\
d d=-e\wedge c-b\wedge f,&d e=-f\wedge a+d\wedge c,&d f=-d\wedge b-a\wedge e.
\end{array}
$$

Define $\alpha_1^\pm=a\pm d$, $\alpha_2^\pm=b\pm e$, and $\alpha_3^\pm=c\pm f$. For example,

$$
d\alpha_1^+=-b\wedge c-e\wedge f-e\wedge c-b\wedge f
=-(b+e)\wedge(c+f).
$$

The minus combination and the other two cyclic combinations give

$$
\boxed{d\alpha_1^\pm=-\alpha_2^\pm\wedge\alpha_3^\pm,\quad
 d\alpha_2^\pm=-\alpha_3^\pm\wedge\alpha_1^\pm,\quad
 d\alpha_3^\pm=-\alpha_1^\pm\wedge\alpha_2^\pm.}
$$

The six forms are independent, since the original pairs are their half-sums and half-differences. Their dual vector fields $E_i^+,E_i^-$ consequently obey

$$
[E_i^\pm,E_j^\pm]=\epsilon_{ijk}E_k^\pm,\qquad [E_i^+,E_j^-]=0.
$$

Each triple is a three-dimensional [Lie algebra ideal](../../../../../ideal-of-a-lie-algebra.md) with the [SO(3) Lie algebra](../../../../../so-3-lie-algebra.md) brackets; the two ideals commute and span the original six-dimensional algebra. This proves the [real four-dimensional rotation algebra splitting](../../../../../real-four-dimensional-rotation-algebra-splitting.md)

$$
\boxed{\mathfrak{so}(4)\cong\mathfrak{so}(3)\oplus\mathfrak{so}(3).}
$$

This is a Lie-algebra statement. Globally $SO(4)$ is a central quotient of $SU(2)\times SU(2)$; a direct product of the corresponding $SO(3)$ groups is not asserted.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
