# Open-loop control

↑ **Parent:** [Control theory](control-theory-split.md)

An [open-loop control](open-loop-control.md) is prescribed as a function of time, possibly after calculation from an initial state and a dynamical model. It is executed without using observations of the actual current state to change the input. A simulated [feedback control](closed-loop-control.md) law can generate an open-loop waveform, but the resulting laboratory control does not automatically correct errors in the actual state or model.

For the ideal [controlled plant](plant-control-theory.md) with $w=0$, plan the [control input](control-input.md)

$$
u(t)=\begin{cases}1,&0\le t<1,\\0,&t\ge1.\end{cases}
$$

[Integration](integral.md) gives $x(t)=\min(t,1)$, so the planned command reaches the [reference signal](reference-signal.md) $r=1$ at $t=1$. If an unplanned constant [control disturbance](control-disturbance.md) $w=0.2$ begins at $t=2$, the same [open-loop control](open-loop-control.md) gives $x(t)=1+0.2(t-2)$ for $t\ge2$: $x(4)=1.4$ and $x(8)=2.2$. Knowing the nominal response did not provide a way to correct the actual [plant output](output-control-theory.md).

## ↑ Ancestors (4)

1. [Control theory](control-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Adaptive experimental quantum control](adaptive-experimental-quantum-control.md)
- [Closed-loop control](closed-loop-control.md)
- [Control theory](control-theory-split.md)
- [Controller (control theory)](controller-control-theory.md)
- [Hamiltonian engineering](hamiltonian-engineering.md)
- [Lyapunov quantum control](lyapunov-quantum-control.md)
- [Open-loop control](open-loop-control.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/1/e/solution.md)
