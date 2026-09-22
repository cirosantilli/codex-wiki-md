<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix the input-index convention

$$
De_i=\sum_j\theta_{ij}\otimes e_j,\qquad D^2e_i=\sum_j\Theta_{ij}\otimes e_j.
$$

Extend the [connection on a vector bundle](../../../../../connection-vector-bundle.md) by the graded [Leibniz rule](../../../../../leibniz-rule.md), $D(\alpha\otimes s)=d\alpha\otimes s+(-1)^{\deg\alpha}\alpha\wedge Ds$. Applying it twice gives

$$
D^2e_i=\sum_jd\theta_{ij}\otimes e_j-\sum_{j,k}\theta_{ij}\wedge\theta_{jk}\otimes e_k,
$$

so

$$
\boxed{\Theta=d\theta-\theta\wedge\theta.}
$$

This is the [Cartan curvature equation with input indices](../../../../../cartan-curvature-equation-with-input-indices.md). In the more usual coefficient-column convention $A=\theta^t$, and $(A\wedge A)^t=-\theta\wedge\theta$ because the entries have degree one. Thus $F=dA+A\wedge A=\Theta^t$; the sign difference is entirely conventional.

The [Chern connection](../../../../../chern-connection.md) of a [Hermitian vector bundle](../../../../../hermitian-vector-bundle.md) with holomorphic structure is characterized by [metric compatibility](../../../../../metric-compatibility.md) and $D^{0,1}=\bar\partial_E$. To construct it, use a [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) and let $h_{ij}=\langle e_i,e_j\rangle$, with the [Hermitian inner product](../../../../../hermitian-form.md) linear in the first variable. The second defining property makes $\theta$ type $(1,0)$. The first gives

$$
dh=\theta h+h\overline\theta^t,\qquad\partial h=\theta h,
$$

and therefore the only possible matrix is

$$
\boxed{\theta=(\partial h)h^{-1}.}
$$

Conversely, this formula has type $(1,0)$ and satisfies both type components of the metric identity, because $h=\overline h^t$. Under a holomorphic frame change $e'=ge$, $h'=gh\overline g^t$ and direct differentiation gives

$$
\theta'=\partial g\,g^{-1}+g\theta g^{-1}.
$$

This is precisely the transformation obtained by differentiating $e'=ge$. The locally constructed connections glue, proving existence, and the forced formula proves uniqueness of the [Chern connection](../../../../../chern-connection.md).

The derivative of $h^{-1}$ gives $\partial\theta=\theta\wedge\theta$. Consequently the [Chern curvature](../../../../../chern-curvature.md) is

$$
\boxed{\Theta=\bar\partial\theta\in A^{1,1}(\operatorname{End}E),\qquad\bar\partial_{\operatorname{End}E}\Theta=0.}
$$

The second assertion is $\bar\partial^2\theta=0$ in a [holomorphic local frame](../../../../../holomorphic-local-trivialization.md); holomorphic transition functions make it intrinsic. Thus the [curvature Dolbeault class](../../../../../curvature-dolbeault-class.md) is $\Psi=[\Theta]\in H^1(M,\Omega_M^1\otimes\operatorname{End}E)$ by the [Dolbeault theorem](../../../../../dolbeault-theorem.md). Here $\Omega^1(\operatorname{End}E)$ denotes this tensor product. We use the identification with bundle-valued Dolbeault forms in which the antiholomorphic exterior factor is placed first, so $\bar\partial\theta$ has the stated positive descent sign.

For the stated transitions $e^{(\beta)}=g_{\alpha\beta}e^{(\alpha)}$, differentiating the frame relation yields

$$
\theta_\beta=g_{\alpha\beta}\theta_\alpha g_{\alpha\beta}^{-1}+(\partial g_{\alpha\beta})g_{\alpha\beta}^{-1}.
$$

Transport the alpha matrix to the beta frame before subtracting it. The difference is the holomorphic section

$$
\boxed{\sigma_{\alpha\beta}=(\partial g_{\alpha\beta})g_{\alpha\beta}^{-1}.}
$$

On a triple intersection, $g_{\alpha\gamma}=g_{\beta\gamma}g_{\alpha\beta}$, so

$$
\sigma_{\alpha\gamma}=\sigma_{\beta\gamma}+g_{\beta\gamma}\sigma_{\alpha\beta}g_{\beta\gamma}^{-1}.
$$

This is exactly the [Čech cocycle condition](../../../../../cech-cocycle-condition.md) after transporting all representatives to the gamma frame.

To identify its class, let $D_\alpha$ be the local holomorphic connection making the alpha frame parallel. Then $t_\alpha=D-D_\alpha$ is a genuine local section of $A^{1,0}(\operatorname{End}E)$, represented by $\theta_\alpha$, with $\bar\partial t_\alpha=\Theta$. Its [Čech coboundary](../../../../../cech-coboundary.md), using $t_\beta-t_\alpha$, is the intrinsic section represented by $\sigma_{\alpha\beta}$ in the beta frame. This local-primitive construction is the Čech–Dolbeault identification, and proves that $(\sigma_{\alpha\beta})$ maps to $\Psi$. For an arbitrary trivializing cover use its natural map to [sheaf cohomology](../../../../../sheaf-cohomology.md); a Stein refinement gives the usual Čech computation. The resulting object is the [Čech cocycle for the curvature Dolbeault class](../../../../../cech-cocycle-for-the-curvature-dolbeault-class.md).

If the metric changes, the difference $B=D'-D$ is a global smooth $(1,0)$ form with values in $\operatorname{End}E$. The local curvature formulas give $\Theta'-\Theta=\bar\partial B$, so $\Psi$ is metric independent. If holomorphic frames change by $e'_\alpha=u_\alpha e_\alpha$, the corresponding local tensors $t'_\alpha-t_\alpha$, expressed in the old frame, are $B_\alpha=u_\alpha^{-1}\partial u_\alpha$. They are holomorphic, and their differences change the cocycle by $\delta B$. Hence **$\Psi$ depends only on the holomorphic bundle, not on its metric or trivializations**.

Apply [exterior product](../../../../../exterior-product.md) and endomorphism composition to curvature to define

$$
\boxed{\Psi^{(k)}=[\Theta^{\wedge k}]\in H^k(M,\Omega_M^k\otimes\operatorname{End}E),\qquad\operatorname{tr}\Psi^{(k)}\in H^k(M,\Omega_M^k).}
$$

These are closed for the [Dolbeault operator](../../../../../dolbeault-operator.md) by the product rule. Their independence can also be verified without commuting matrices. If $\Theta_1-\Theta_0=\bar\partial B$, then

$$
\Theta_1^k-\Theta_0^k=\bar\partial\left(\sum_{j=0}^{k-1}\Theta_1^j\wedge B\wedge\Theta_0^{k-1-j}\right).
$$

This follows by the noncommutative telescoping identity and the even total degree of curvature. The matrix products are interpreted in the fixed frame convention; powers of the degree-two curvature transpose to the corresponding usual curvature powers. The trace contraction is invariant under frame changes, so its class is well defined. This proves [metric independence of curvature Dolbeault powers](../../../../../metric-independence-of-curvature-dolbeault-powers.md); for $k>\dim M$ the forms and groups in question vanish.

Finally take a smooth unitary frame. Metric compatibility gives $\theta^\dagger=-\theta$, and the [Cartan curvature equation with input indices](../../../../../cartan-curvature-equation-with-input-indices.md) gives $\Theta^\dagger=-\Theta$. Thus

$$
\overline{\operatorname{tr}(\Theta^k)}=(-1)^k\operatorname{tr}(\Theta^k),\qquad \overline{\left(\frac{i}{2\pi}\right)^k\operatorname{tr}(\Theta^k)}=\left(\frac{i}{2\pi}\right)^k\operatorname{tr}(\Theta^k).
$$

The second expression is therefore a real differential form. It is also $d$-closed: differentiating Cartan's equation gives $d\Theta=\theta\wedge\Theta-\Theta\wedge\theta$, and cyclicity of trace cancels the resulting commutator in $d\operatorname{tr}(\Theta^k)$. On a compact [Kähler manifold](../../../../../kahler-manifold.md), the [Hodge decomposition theorem for compact Kähler manifolds](../../../../../hodge-decomposition-theorem-for-compact-kahler-manifolds.md) identifies $H^k(M,\Omega_M^k)$ with the $(k,k)$ component of complex [de Rham cohomology](../../../../../de-rham-cohomology.md). Hence

$$
\boxed{\left(\frac{i}{2\pi}\right)^k\operatorname{tr}(\Psi^{(k)})\text{ determines a class in }H^{2k}_{\mathrm{DR}}(M,\mathbb R).}
$$

It is $k!$ times the degree-$2k$ component of the [Chern character](../../../../../chern-character.md). Reality does not assert integrality of these individual power-sum classes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
