<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For constant [alpha tensor](../../../../../alpha-tensor.md) and positive [magnetic diffusivity](../../../../../magnetic-diffusivity.md) $\eta$, the steady [anisotropic alpha-squared dynamo](../../../../../anisotropic-alpha-squared-dynamo.md) equation is

$$
0=\nabla\times(\boldsymbol\alpha\mathbf B)+\eta\nabla^2\mathbf B,
\qquad\nabla\cdot\mathbf B=0.
$$

For a nonzero [Fourier mode](../../../../../fourier-mode.md) with wavevector $\mathbf K=(k,l,m)$, this becomes $\eta K^2\mathbf B=i\mathbf K\times(\boldsymbol\alpha\mathbf B)$. Rotational symmetry of the [alpha tensor](../../../../../alpha-tensor.md) in the horizontal plane lets us set $\mathbf K=(q,0,m)$, with $q^2=k^2+l^2$. The component equations are

$$
\eta K^2B_x=-im\alpha_0B_y,\qquad
\eta K^2B_y=i(m\alpha_0B_x-q\alpha_1B_z),\qquad
\eta K^2B_z=iq\alpha_0B_y.
$$

Substitute the first and third into the second. A nonzero steady amplitude requires $\eta^2K^4=\alpha_0^2m^2+\alpha_0\alpha_1q^2$. Conversely, this relation supplies a nonzero amplitude through the same component equations, and the [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md) $qB_x+mB_z=0$ is automatically satisfied. Thus **the steady-mode condition is**

$$
\boxed{(q^2+m^2)^2=\gamma^2(m^2+\delta q^2),\qquad
\gamma^2=\frac{(q^2+m^2)^2}{m^2+\delta q^2}.}
$$

For the first form, no division by $m^2+\delta q^2$ is needed. The quotient applies when that denominator is nonzero, in particular for $q>0$ and $0<\delta<1$.

Put $Q=q^2>0$ and $r=m^2\geq0$. The derivative of $F(r)=(Q+r)^2/(r+\delta Q)$ is

$$
F'(r)=\frac{(Q+r)[r+(2\delta-1)Q]}{(r+\delta Q)^2}.
$$

For $0<\delta<1/2$, the derivative changes from negative to positive at $r=(1-2\delta)Q$. For $1/2\leq\delta<1$ it is nonnegative throughout the allowed half-line and the minimum is at $r=0$. Therefore **the optimized [uniaxial alpha dynamo threshold](../../../../../uniaxial-alpha-dynamo-threshold.md) is**

$$
\boxed{
\begin{aligned}
0<\delta<\tfrac12:\quad &m_*^2=(1-2\delta)q^2,\qquad\gamma_{\min}^2=4(1-\delta)q^2,\\
\tfrac12\leq\delta<1:\quad &m_*^2=0,\qquad\gamma_{\min}^2=q^2/\delta.
\end{aligned}}
$$

Both expressions agree at $\delta=1/2$. If the horizontal boundary conditions permit $q=0$, a nonzero mode instead has $\gamma^2=m^2$ and the infimum is zero as $m\to0$; it is not attained by a nonzero wavevector. The exactly uniform mode $q=m=0$ has no diffusive or alpha curl term and must be treated separately.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
