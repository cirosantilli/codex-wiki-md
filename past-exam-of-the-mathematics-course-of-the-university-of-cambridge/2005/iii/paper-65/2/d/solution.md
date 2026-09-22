<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On $a+2b=1$ the coexistence [fixed point](../../../../../../fixed-point.md) has

$$
D=1,\qquad T=\frac{5a-1}{2a},\qquad
\cos\theta=\frac{5a-1}{4a}.
$$

For $1/9<a<1$ these give a nonreal conjugate pair on the [unit circle](../../../../../../complex-unit-circle.md). Nearby, while the pair remains complex, its modulus is $\sqrt D$; increasing $a+2b$ through one changes the modulus from greater than one to less than one. This is the candidate [Neimark–Sacker bifurcation](../../../../../../neimark-sacker-bifurcation.md), and a nonlinear coefficient is needed to decide its direction.

Here that coefficient can be calculated explicitly. Let $\rho=e^{i\theta}$, $\sigma=\sin\theta>0$, and normalize the right [eigenvector](../../../../../../eigenvector.md) and complex projection by

$$
q=\begin{pmatrix}1\\-1/(2a)-i\sigma/b\end{pmatrix},\qquad
p=\left(\frac12+\frac{ib}{4a\sigma},\frac{ib}{2\sigma}\right),\qquad pq=1,\quad p\overline q=0.
$$

For deviations $(X,Y)=zq+\overline z\,\overline q$, the quadratic derivative is

$$
\mathcal B(v,w)=\begin{pmatrix}
-2v_1w_1/a-v_1w_2-v_2w_1\\
(v_1w_2+v_2w_1)/b
\end{pmatrix}.
$$

Thus $f_{20}=p\mathcal B(q,q)/2$, $f_{11}=p\mathcal B(q,\overline q)$ and $f_{02}=p\mathcal B(\overline q,\overline q)/2$ are the quadratic coefficients in $z'$. The quadratic coordinate change has

$$
h_{20}=\frac{f_{20}}{\rho^2-\rho},\quad
h_{11}=\frac{f_{11}}{1-\rho},\quad
h_{02}=\frac{f_{02}}{\overline\rho^2-\rho}.
$$

Substitution into the map and collection of $w^2\overline w$ yields

$$
g_{21}=2f_{20}h_{11}+f_{11}h_{20}+f_{11}\overline h_{11}+2f_{02}\overline h_{02}.
$$

Using $b=(1-a)/2$ and $\sigma^2=(1-a)(9a-1)/(16a^2)$ simplifies the [cubic radial coefficient of a quadratic planar map](../../../../../../cubic-radial-coefficient-of-a-quadratic-planar-map.md) to

$$
\boxed{\ell=\operatorname{Re}(\overline\rho g_{21})=-\frac1{a^2(1-a)}<0.}
$$

Consequently, away from [strong resonances of a planar map](../../../../../../strong-resonance-of-a-planar-map.md), the bifurcation is supercritical: on $a+2b>1$ coexistence is attracting, whereas on $a+2b<1$ a small attracting invariant closed curve surrounds the unstable coexistence [fixed point](../../../../../../fixed-point.md). If $\eta=\sqrt D-1>0$, its leading radius is $|w|^2=-\eta/\ell$, and its radial multiplier is $1-2\eta+\cdots$. Motion on the curve can be quasiperiodic or frequency-locked into periodic motion; stability of the curve alone does not imply an irrational rotation.

Two interior values need qualification: **$a=1/7$ is a 1:3 resonance, and $a=1/5$ is a 1:4 resonance**. At the former $h_{02}$ is singular and the quadratic $\overline w^2$ term must be retained. At the latter a cubic $\overline w^3$ term remains. The resonant terms can be displayed explicitly in the same normalization. At $a=1/7$, $f_{02}=-7/6-7\sqrt3\,i/2\ne0$. The third iterate, near the resonance and after removing nonresonant quadratics, has

$$
F^3(w)-w=3(\eta+i\delta)w+3\overline\rho f_{02}\overline w^2+\cdots.
$$

Here $\delta$ is the angular detuning. Its nonzero stationary solutions have $|w|=\sqrt{\eta^2+\delta^2}/|f_{02}|$ and three phases; they constitute a saddle three-cycle. Indeed the two leading real exponents at these solutions are $3[\eta\pm\sqrt{4\eta^2+3\delta^2}]$, of opposite signs. Therefore no ordinary attracting-circle conclusion follows arbitrarily close to the exact 1:3 point.

At $a=1/5$, the cubic resonant [normal form](../../../../../../normal-form-dynamical-systems.md) is

$$
w'=i\big[(1+\eta+i\delta)w+g w|w|^2+h\overline w^3\big]+\cdots,
\qquad g=-\frac{125}{4}+\frac{125}{8}i,\quad h=-25+\frac{25}{8}i.
$$

The extra coefficient follows from $g_{03}=f_{11}h_{02}+2f_{02}\overline h_{20}$ and $h=\overline\rho g_{03}$. Its radial cubic damping is uniform since $\operatorname{Re}g+|h|<0$. The slow angular equation is $\Delta\arg w=\delta+|w|^2\operatorname{Im}(g+he^{-4i\arg w})+\cdots$, so fourfold phase locking must be considered. For example, varying $b$ at fixed $a=1/5$ gives $\delta=-\eta/2+\cdots$. The locked branches satisfy $\tan(4\arg w)=6/17$ and $|w|^2=-\eta/\operatorname{Re}(g+he^{-4i\arg w})$. For $\eta>0$ they form one attracting and one saddle four-cycle; the two branches alternate in phase. This is a resonant alternative to quasiperiodic motion on an invariant curve. The endpoints also fail the simple-complex-pair assumptions. This distinguishes the generic nearby dynamics from unjustified claims about every point on the printed interval.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
