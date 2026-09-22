<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $L\alpha=\omega\wedge\alpha$, the [Lefschetz operator of a Kähler manifold](../../../../../lefschetz-operator-of-a-kahler-manifold.md). The metric and volume form define the $L^2$ [inner product](../../../../../inner-product.md) on smooth complex forms, and $\Lambda=L^*$ is its [formal adjoint](../../../../../formal-adjoint.md). Similarly, $\bar\partial^*$ is the [formal adjoint](../../../../../formal-adjoint.md) of the [Dolbeault operator](../../../../../dolbeault-operator.md), characterized by $\langle\bar\partial\beta,\alpha\rangle=\langle\beta,\bar\partial^*\alpha\rangle$. The [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) is

$$
 \boxed{\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.}
$$

On the compact manifold without boundary, integration by parts gives

$$
 \langle\Delta_{\bar\partial}\alpha,\alpha\rangle
 =\|\bar\partial\alpha\|_2^2+\|\bar\partial^*\alpha\|_2^2.
$$

If the Laplacian vanishes, both terms are zero. Conversely, if both operators annihilate $\alpha$, the defining formula annihilates it. Thus **harmonicity is equivalent to being both $\bar\partial$-closed and $\bar\partial^*$-closed**.

Because $\omega$ is closed and has type $(1,1)$, $\bar\partial\omega=0$ and $[L,\bar\partial]=0$. The supplied identity from the [Kähler identities](../../../../../kahler-identities.md) gives $[L,\bar\partial^*]=-i\partial$. With ordinary commutators for the even-degree operator $L$,

$$
 \begin{aligned}
 [L,\Delta_{\bar\partial}]&=[L,\bar\partial]\bar\partial^*
 +\bar\partial[L,\bar\partial^*]+[L,\bar\partial^*]\bar\partial
 +\bar\partial^*[L,\bar\partial]\\
 &=-i(\bar\partial\partial+\partial\bar\partial)=0.
 \end{aligned}
$$

The last identity follows from $d^2=0$. This also proves that the Lefschetz operator preserves harmonic forms.

For the cohomology map one can work directly with forms: $\bar\partial(\omega^k\wedge\alpha)=\omega^k\wedge\bar\partial\alpha$, since $\omega$ has even degree. It takes closed forms to closed forms and exact forms to exact forms. Therefore the $k$th power of $L$ induces

$$
 \boxed{\phi_{\omega,k}([\alpha])=[\omega^k\wedge\alpha].}
$$

The bidegree is $(p+k,q+k)$, including the zero groups outside the dimension range. No isomorphism claim is needed here.

Finally put $\theta=-i\partial f$, so $\bar\partial\theta=i\partial\bar\partial f=\omega'-\omega$. Let

$$
 T_k=\sum_{j=0}^{k-1}(\omega')^j\wedge\omega^{k-1-j}.
$$

Both [Kähler forms](../../../../../kahler-form.md) are $\bar\partial$-closed, so $\bar\partial T_k=0$. For a closed representative $\alpha$,

$$
 (\omega')^k\wedge\alpha-\omega^k\wedge\alpha
 =\bar\partial\bigl(\theta\wedge T_k\wedge\alpha\bigr).
$$

This primitive has type $(p+k,q+k-1)$; the degree-one sign produces no additional term because $T_k\wedge\alpha$ is closed. Hence

$$
 \boxed{\phi_{\omega,k}=\phi_{\omega',k}\quad\text{for every }k\geq1.}
$$

This is the [dependence of Lefschetz maps on the Dolbeault class](../../../../../dependence-of-lefschetz-maps-on-the-dolbeault-class.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
