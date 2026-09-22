<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Lie algebra representation](../../../../../lie-algebra-representation.md) is a linear map $\rho:\mathfrak g\to\operatorname{End}(V)$ preserving brackets: $\rho([X,Y])=[\rho(X),\rho(Y)]$. Differentiating a smooth [unitary representation](../../../../../unitary-representation.md) $D$ of a [Lie group](../../../../../lie-group.md) gives $\rho(X)=\left.\frac{d}{dt}D(e^{tX})\right|_{t=0}$, an anti-Hermitian operator for each real algebra element $X$. In the physics convention one uses Hermitian generators $t_X=i\rho(X)$ and writes $D(e^{tX})=e^{-it t_X}$. Conversely, [integration of a Lie-algebra representation](../../../../../integration-of-a-lie-algebra-representation.md) gives a representation of the connected simply connected group. A representation of another group with the same algebra additionally has to be trivial on the kernel of its [covering map](../../../../../covering-space.md).

For the [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md), take $J_3$ Hermitian and $J_+^\dagger=J_-$ on a positive-definite inner-product space. A [highest-weight vector](../../../../../highest-weight-vector.md) has $J_3|j,j\rangle=j|j,j\rangle$ and $J_+|j,j\rangle=0$. Set $v_\ell=(J_-)^\ell|j,j\rangle$. Commuting $J_3$ through each lowering operator gives $J_3v_\ell=(j-\ell)v_\ell$. Furthermore,

$$
[J_+,(J_-)^\ell]=\sum_{r=0}^{\ell-1}(J_-)^r(2J_3)(J_-)^{\ell-1-r},
$$

so acting on the highest-weight state and summing the coefficients gives

$$
J_+v_\ell=\ell(2j-\ell+1)v_{\ell-1}.
$$

Taking the [inner product](../../../../../inner-product.md) with $v_{\ell-1}$ produces the [unitary highest-weight termination](../../../../../unitary-highest-weight-termination.md) recursion

$$
\|v_\ell\|^2=\ell(2j-\ell+1)\|v_{\ell-1}\|^2.
$$

The first factor requires $j\ge0$. If $2j$ is not an integer, the first integer $\ell>2j+1$ would make the norm negative, while every preceding norm is positive. Thus

$$
\boxed{2j\in\mathbb Z_{\ge0}.}
$$

For these values, $v_0,\ldots,v_{2j}$ have strictly positive norms and distinct [eigenvalues](../../../../../eigenvalue.md), while $v_{2j+1}$ has zero norm and hence is zero. They therefore span a space of [dimension](../../../../../dimension-vector-space.md) $2j+1$, invariant under all three generators. Its weights are $j,j-1,\ldots,-j$. This proves **integer or half-integer [spin](../../../../../spin.md) and finite [dimension](../../../../../dimension-vector-space.md) $2j+1$**. The positive-definite unitary assumption matters: an unrestricted algebraic highest-weight module need not terminate. Normalizing the ladder states yields

$$
J_\pm|j,m\rangle=\sqrt{(j\mp m)(j\pm m+1)}\,|j,m\pm1\rangle.
$$

This is the [normalized highest-weight lowering formula](../../../../../normalized-highest-weight-lowering-formula.md) with the usual positive ladder phases and units $\hbar=1$.

In the ordered spin-one-half basis $(|1/2,1/2\rangle,|1/2,-1/2\rangle)$, the matrices are

$$
\boxed{J_3=\frac12\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad
J_+=\begin{pmatrix}0&1\\0&0\end{pmatrix},\quad
J_-=\begin{pmatrix}0&0\\1&0\end{pmatrix}.}
$$

Thus $J_i=\sigma_i/2$, where the $\sigma_i$ are [Pauli matrices](../../../../../pauli-matrices.md).

Choose the active-rotation convention. The [SU(2)](../../../../../su-2-group.md) lift of an axis-angle rotation is

$$
U_{1/2}(\vartheta,\mathbf n)=e^{-i\vartheta\mathbf n\cdot\boldsymbol\sigma/2}
=\cos(\vartheta/2)I-i\sin(\vartheta/2)\mathbf n\cdot\boldsymbol\sigma.
$$

The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) shows that conjugating $\mathbf x\cdot\boldsymbol\sigma$ by this [matrix](../../../../../matrix.md) produces $(R\mathbf x)\cdot\boldsymbol\sigma$, with

$$
R\mathbf x=\mathbf x\cos\vartheta+(\mathbf n\times\mathbf x)\sin\vartheta
+\mathbf n(\mathbf n\cdot\mathbf x)(1-\cos\vartheta).
$$

This is the ordinary three-dimensional rotation. In any spin-$j$ representation the corresponding unitary operator and its [matrix](../../../../../matrix.md) elements are

$$
\boxed{U_j(R)=e^{-i\vartheta\mathbf n\cdot\mathbf J^{(j)}},\qquad
D^{(j)}_{mm'}(R)=\langle j,m|U_j(R)|j,m'\rangle.}
$$

For half-integer [spin](../../../../../spin.md), $R$ in this notation includes a choice of lift to [SU(2)](../../../../../su-2-group.md); it does not define a single-valued representation of [SO(3)](../../../../../so-3-group.md).

For the specified Euler-angle order, the rightmost rotation acts first:

$$
\boxed{U_j(R)=e^{-i\phi J_3}e^{-i\theta J_2}e^{-i\psi J_3},\qquad
D^{(j)}_{mm'}(R)=e^{-im\phi}d^{(j)}_{mm'}(\theta)e^{-im'\psi}.}
$$

Here the [Wigner D-matrix](../../../../../wigner-d-matrix.md) middle factor is $d^{(j)}_{mm'}(\theta)=\langle j,m|e^{-i\theta J_2}|j,m'\rangle$. It can be calculated explicitly by realizing [spin](../../../../../spin.md) $j$ as the symmetric product of $2j$ spin-one-half factors. Write $c=\cos(\theta/2)$ and $s=\sin(\theta/2)$. The fundamental rotation sends $|+\rangle$ to $c|+\rangle+s|-\rangle$ and $|-\rangle$ to $-s|+\rangle+c|-\rangle$. Expanding a normalized symmetric state with $j+m'$ plus signs gives

$$
d^{(j)}_{mm'}(\theta)=\sqrt{(j+m)!(j-m)!(j+m')!(j-m')!}
\sum_r\frac{(-1)^{m-m'+r}c^{2j+m'-m-2r}s^{m-m'+2r}}
{(j+m'-r)!\,r!\,(m-m'+r)!\,(j-m-r)!},
$$

where $\max(0,m'-m)\le r\le\min(j+m',j-m)$. The exponent $r$ counts initially positive spinors that become negative, while $m-m'+r$ counts initially negative ones that become positive; their minus signs and binomial coefficients give the displayed expression. Every factorial argument is an integer even for half-integer [spin](../../../../../spin.md).

For [spin](../../../../../spin.md) one-half this reduces to the explicit [matrix](../../../../../matrix.md)

$$
D^{(1/2)}(\phi,\theta,\psi)=
\begin{pmatrix}
e^{-i(\phi+\psi)/2}\cos(\theta/2)&-e^{-i(\phi-\psi)/2}\sin(\theta/2)\\
e^{i(\phi-\psi)/2}\sin(\theta/2)&e^{i(\phi+\psi)/2}\cos(\theta/2)
\end{pmatrix}.
$$

Replacing $\theta$ by $\theta+2\pi$ reverses both sine and cosine, so every entry changes sign. In particular, a pure $2\pi$ rotation gives **$D^{(1/2)}=-I$**, while a $4\pi$ rotation gives $I$.

Finally, the [Adjoint double cover from SU(2) to SO(3)](../../../../../adjoint-double-cover-from-su-2-to-so-3.md) is surjective by the axis-angle construction. Its kernel consists of matrices commuting with all Pauli matrices, hence scalar matrices; within [SU(2)](../../../../../su-2-group.md) these are $\pm I$. Thus

$$
\boxed{SO(3)\cong SU(2)/\{\pm I\}.}
$$

Their [Lie algebras](../../../../../lie-algebra-split.md) are isomorphic, but their global topology and representations differ. In [spin](../../../../../spin.md) $j$, the central element $-I$ acts as $(-1)^{2j}I$, so exactly the integer-spin representations descend to ordinary [SO(3)](../../../../../so-3-group.md) representations. This is the [descent of an SU(2) representation to SO(3)](../../../../../descent-of-an-su-2-representation-to-so-3.md) criterion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
