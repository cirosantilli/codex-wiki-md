<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

[Faraday's law of induction](../../../faraday-s-law-of-induction.md) states that the oriented [electromotive force](../../../electromotive-force.md) around a closed material circuit is minus the rate of change of its linked [magnetic flux](../../../magnetic-flux.md):

$$
\mathcal E=\oint_{C(t)}(\mathbf E+\mathbf u\times\mathbf B)\cdot d\boldsymbol\ell
=-\frac{d}{dt}\int_{S(t)}\mathbf B\cdot d\mathbf S.
$$

The surface orientation and circuit direction obey the [right-hand rule](../../../right-hand-rule.md). The minus sign expresses [Lenz's law](../../../lenz-s-law.md): the induced [electric current](../../../electric-current.md), when allowed to flow, produces a [magnetic field](../../../magnetic-field-split.md) opposing the change of linked [magnetic flux](../../../magnetic-flux.md). For a stationary circuit this reduces to $\oint\mathbf E\cdot d\boldsymbol\ell=-d\Phi_B/dt$.

The source's “Lorenz force” is the [Lorentz force](../../../lorentz-force.md), $q(\mathbf E+\mathbf v\times\mathbf B)$. A wire element of cross-section $A_c$ contains $nA_c\,d\ell$ carriers of charge $q$ with drift [velocity](../../../velocity.md) $\mathbf v_d$. Adding their magnetic [forces](../../../force-split.md) and using $I=nqA_cv_d$ gives

$$
\boxed{d\mathbf F=I\,d\boldsymbol\ell\times\mathbf B,\qquad
\mathbf F=I\mathbf L\times\mathbf B}
$$

for a straight wire in a uniform [magnetic field](../../../magnetic-field-split.md). The length [vector](../../../vector.md) follows conventional [electric current](../../../electric-current.md), irrespective of the carrier sign.

For the unlabelled upward-motion request, define $\hat{\mathbf t}=(\cos\phi,0,-\sin\phi)$ down the slope, $\hat{\mathbf b}=(0,1,0)$ across the rails and $\hat{\mathbf n}=(\sin\phi,0,\cos\phi)$ out of their plane. Choose the vertical [magnetic field](../../../magnetic-field-split.md) as $\mathbf B=B\hat{\mathbf z}$. An [electric current](../../../electric-current.md) $I$ across the bar in direction $-\hat{\mathbf b}$ gives a horizontal [magnetic force](../../../magnetic-force.md) $-IBs\hat{\mathbf x}$. The other [forces](../../../force-split.md) are weight $-mg\hat{\mathbf z}$ and the rail [normal force](../../../normal-force.md) $N\hat{\mathbf n}$. Uniform upward [velocity](../../../velocity.md) requires

$$
mg\sin\phi-IBs\cos\phi=0,\qquad
N-mg\cos\phi-IBs\sin\phi=0.
$$

Consequently

$$
\boxed{I=\frac{mg\tan\phi}{Bs},\qquad
F_B=\frac{mg\sin\phi}{\cos\phi},\qquad N=\frac{mg}{\cos\phi}.}
$$

Each symmetric rail supplies half of $N$. The [electric current](../../../electric-current.md) must make $I\mathbf L\times\mathbf B$ point horizontally toward the uphill side; for the coordinates just defined it flows along $-\hat{\mathbf b}$. Reversing the vertical [magnetic field](../../../magnetic-field-split.md) reverses this current direction. The external supply must maintain that [electric current](../../../electric-current.md) against the motional [electromotive force](../../../electromotive-force.md) during ascent. For $\cos\phi=0$, no finite horizontal [magnetic force](../../../magnetic-force.md) can support uniform motion along the vertical rails.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
