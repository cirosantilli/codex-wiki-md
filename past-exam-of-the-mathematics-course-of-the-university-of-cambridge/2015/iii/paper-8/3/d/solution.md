<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For positive smooth $f$ with the stated decay, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\boxed{\int f''\log f\,dv=-\int\frac{|f'|^2}{f}\,dv}
$$

and, using unit [mass](../../../../../../mass.md),

$$
\boxed{\int(fv)'\log f\,dv=-\int vf'\,dv=\int f\,dv=1.}
$$

For zero values of $f$, these calculations can be made with the positive unit-mass approximation $(f+\varepsilon\gamma)/(1+\varepsilon)$ and then passed to the limit whenever the quantities are finite. Positive-time solutions also have the usual Gaussian smoothing.

Since $-\log\gamma=v^2/2+\tfrac12\log(2\pi)$, [mass](../../../../../../mass.md) conservation gives

$$
H(f_t\mid\gamma)=\int f_t\log f_t\,dv+
\frac12\int v^2f_t\,dv+\frac12\log(2\pi).
$$

The derivative of the first term is $\int\partial_tf_t\log f_t$, because $\int\partial_tf_t=0$. The two identities above and the [energy](../../../../../../energy.md) equation in (b), with $d=M=1$, yield

$$
\frac d{dt}H(f_t\mid\gamma)
=-\int\frac{|f_t'|^2}{f_t}\,dv+1+
\left(1-\int v^2f_t\,dv\right).
$$

Now expand the [relative Fisher information](../../../../../../relative-fisher-information.md):

$$
I(f\mid\gamma)=\int\left|\partial_v\log(f/\gamma)\right|^2f\,dv
=\int\left(\frac{f'}f+v\right)^2f\,dv
=\int\frac{|f'|^2}{f}\,dv+\int v^2f\,dv-2,
$$

where $\int vf'=-1$. **Thus the [entropy dissipation identity for Ornstein-Uhlenbeck flow](../../../../../../entropy-dissipation-identity-for-ornstein-uhlenbeck-flow.md) is**

$$
\boxed{\frac d{dt}H(f_t\mid\gamma)=-I(f_t\mid\gamma)\leq0.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
