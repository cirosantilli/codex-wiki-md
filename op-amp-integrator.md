# Op amp integrator

↑ **Parent:** [Operational amplifier](operational-amplifier.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Op_amp_integrator)

An [op amp integrator](op-amp-integrator.md) places a [resistor](resistor.md) $R$ between the input source and the inverting input of an [operational amplifier](operational-amplifier.md), and a feedback [capacitor](capacitor.md) $C$ between that input and the output, with the non-inverting input grounded. For an [ideal operational amplifier](ideal-operational-amplifier.md), [Kirchhoff's current law](kirchhoff-node-law.md) gives $v_{\mathrm{in}}/R=-C\,dv_o/dt$, hence

$$
v_o(t)=v_o(t_0)-\frac1{RC}\int_{t_0}^t v_{\mathrm{in}}(u)\,du,\qquad H(s)=-\frac1{sRC}.
$$

The initial capacitor charge supplies the integration constant. A parallel feedback [resistor](resistor.md) $R_f$ replaces the transfer by $H(s)=-(R_f/R)/(1+sR_fC)$: the direct-current gain becomes finite while integration is recovered when $|sR_fC|\gg1$. This limits offset-driven saturation. [Analog Devices, Chapter 2, integrator and parallel feedback resistance](https://wiki.analog.com/university/courses/electronics/text/chapter-2)

**Table of contents**

- [Finite-gain operational-amplifier integrator](finite-gain-operational-amplifier-integrator.md)

## ↑ Ancestors (7)

1. [Operational amplifier](operational-amplifier.md)
2. [Electronic amplifier](electronic-amplifier.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Finite-gain operational-amplifier integrator](finite-gain-operational-amplifier-integrator.md)
- [Input bias current](input-bias-current.md)
- [Input offset voltage](input-offset-voltage.md)
- [Op amp integrator](op-amp-integrator.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-2/section-d/d13/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d12/b/solution.md)
