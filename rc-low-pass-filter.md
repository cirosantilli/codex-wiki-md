# RC low-pass filter

↑ **Parent:** [Low-pass filter](low-pass-filter.md)

An RC low-pass filter places a [resistor](resistor.md) $R>0$ between [input](input-computer-science.md) and [output](output-computing.md), with a [capacitor](capacitor.md) $C>0$ from [output](output-computing.md) to their common return. The ideal model prescribes the input [electric potential difference](electric-potential-difference.md) and leaves the output unloaded. It is a [first-order low-pass filter](first-order-low-pass-filter.md) with unit eventual gain.[Lab 3: Filters, §5.4: RC topology and voltage transfer](lab-3-filters-by-university-of-colorado-boulder-physics-undergraduate-labs.md)

<a id="image-rc-low-pass-filter-topology-and-an-optional-electrical-load"></a>
![](rc-low-pass-circuit-and-loading.png)

**[Figure 20](#image-rc-low-pass-filter-topology-and-an-optional-electrical-load). RC low-pass filter topology and an optional electrical load**. Original schematic: the [output](output-computing.md) is across the [capacitor](capacitor.md), not across the [resistor](resistor.md). The orange dashed [resistor](resistor.md) is the optional [electrical load](electrical-load.md) $R_L$ used in [RC low-pass output loading](rc-low-pass-output-loading.md); omit it for the ideal unloaded model. The blue arrow defines positive [electric current](electric-current.md) through $R$.

For [electrical resistance](electrical-resistance.md) $R$ and [capacitance](capacitance.md) $C$, [Ohm's law](ohm-s-law.md) gives the [electric current](electric-current.md) through the [resistor](resistor.md) as $(v_{\rm in}-v_{\rm out})/R$. The [capacitor](capacitor.md) relation gives $C\,dv_{\rm out}/dt$. Equating them by [Kirchhoff's current law](kirchhoff-node-law.md) yields the [ordinary differential equation](ordinary-differential-equation.md)

$$
RC\frac{dv_{\rm out}}{dt}+v_{\rm out}=v_{\rm in},\qquad \tau=RC.
$$

The [time constant](time-constant.md) $\tau$ has units of time. A rapid change in [electric potential difference](electric-potential-difference.md) requires a large [electric current](electric-current.md) into the [capacitor](capacitor.md); the finite [electrical resistance](electrical-resistance.md) limits that rate. A slowly maintained voltage instead lets the [capacitor](capacitor.md) approach the input voltage. The same equation therefore predicts both smoothing of sustained oscillations and a rounded response to a sudden change.

For the original constructed example throughout this article, take

$$
R=2.2\,\mathrm{k}\Omega,\qquad C=47\,\mathrm{nF},\qquad \tau=103.4\,\mu\mathrm{s}.
$$

These stipulated ideal values specify an analytical model, rather than measurements of particular components.

**Table of contents**

- [RC low-pass frequency response](rc-low-pass-frequency-response.md)
- [RC low-pass step response](rc-low-pass-step-response.md)
- [RC low-pass output loading](rc-low-pass-output-loading.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)

## ↑ Ancestors (5)

1. [Low-pass filter](low-pass-filter.md)
2. [Linear filter](linear-filter.md)
3. [Signal processing](signal-processing.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Effective noise bandwidth](effective-noise-bandwidth.md)
- [Low-pass filter](low-pass-filter.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a3/solution.md)
- [RC low-pass filter](rc-low-pass-filter.md)
- [RC low-pass frequency response](rc-low-pass-frequency-response.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [RC low-pass step response](rc-low-pass-step-response.md)
- [Resistor-capacitor equilibrium noise](resistor-capacitor-equilibrium-noise.md)
