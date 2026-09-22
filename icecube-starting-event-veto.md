# IceCube starting-event veto

↑ **Parent:** [IceCube Neutrino Observatory](icecube-neutrino-observatory.md)

The 2013 selection rejected early boundary light. Tagged [muons](muon.md) checked leakage; [air shower](air-shower.md) companion [muons](muon.md) also vetoed downward [atmospheric neutrinos](atmospheric-neutrino.md).[Event Selection; Atmospheric Muon Background](evidence-for-high-energy-extraterrestrial-neutrinos-at-the-icecube-detector-by-icecube-collaboration.md)

<a id="image-entering-tracks-contained-interactions-and-an-accompanying-muon-veto"></a>
![](icecube-contained-event-veto.png)

**[Figure 7](#image-entering-tracks-contained-interactions-and-an-accompanying-muon-veto). Entering tracks, contained interactions and an accompanying-muon veto**. Original schematic, not to scale or measured data. Dots: optical modules. Dashed arrows: unseen neutrinos; solid arrows: muons.

A simple original [conditional probability](conditional-probability.md) model explains why a veto changes the selected mixture. Let $A$ mean that an [atmospheric neutrino](atmospheric-neutrino.md) interaction would pass all other cuts, $M$ that an accompanying [muon](muon.md) reaches the veto, and $V$ that the veto fires. Set $a=P(M\mid A)$ and $\epsilon=P(V\mid M,A)$, and neglect unrelated veto hits. The [law of total probability](law-of-total-probability.md) gives

$$
P(\text{passes veto}\mid A)=1-a\epsilon.
$$

For chosen $a=0.8$ and $\epsilon=0.95$, the passing fraction is $0.24$. Neither this value nor either input is an [IceCube](icecube-neutrino-observatory.md) measurement. With equal incident candidate populations, this mechanism alone reduces the atmospheric contribution relative to a hypothetical population having $a=0$. It does not make every surviving event astronomical: $a=0$ or $\epsilon=0$ gives no suppression, while $a=\epsilon=1$ removes the entire chosen atmospheric population. If unrelated light vetoes a surviving event independently with [probability](probability.md) $u$, its passing fraction becomes $(1-u)(1-a\epsilon)$; independence is an additional assumption.

## ↑ Ancestors (6)

1. [IceCube Neutrino Observatory](icecube-neutrino-observatory.md)
2. [Cherenkov detector](cherenkov-detector.md)
3. [Particle detector](particle-detector.md)
4. [Particle detection](particle-detection-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
