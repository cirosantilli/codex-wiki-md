# Coincidence and noise controls for GW150914

↑ **Parent:** [GW150914](gw150914.md)

The modeled [matched filter](matched-filter.md) search found an arrival difference of about $7\,\mathrm{ms}$, within the roughly $10\,\mathrm{ms}$ intersite light travel time. Background events were obtained by shifting one detector's timestamps far beyond that time and repeating the coincidence analysis. The binary search bounded the [false alarm rate](false-alarm-rate.md) below one event per $203\,000$ years. That is an empirically estimated background rate, not a probability that the source interpretation is false.[Abstract; I Introduction; time-shift background analysis, Fig. 5](gw150914-first-results-from-the-search-for-binary-black-hole-coalescence-with-advanced-ligo-by-b-p-abbott-and-others.md)

The logic is to destroy a common astronomical arrival while retaining each instrument's real glitches. A [Poisson distribution](poisson-distribution.md) approximation would turn a background rate $r$ into $1-e^{-rT}$ for at least one equally strong noise event during live time $T$, only after accounting for the search's ranking and trials. Repeated time slides reuse data; their accumulated background duration is not an equally long series of independent new observations. Correlated disturbances also require separate controls because shifting timestamps can erase them along with a true signal.

The dedicated noise study inspected auxiliary channels and deliberately applied magnetic, acoustic and mechanical disturbances to measure their coupling into strain. For [GW150914](gw150914.md), checks included environmental coincidences, instrument state, and exclusion of an intentional hardware injection. It also examined potentially correlated global magnetic disturbances, which time slides alone cannot exclude.[2 Identifying noise sources, Fig. 2; 6 Validation of GW150914; Appendix B physical environment monitors](characterization-of-transient-noise-in-advanced-ligo-relevant-to-gravitational-wave-signal-gw150914-by-b-p-abbott-and-others.md) The point of an injection test is quantitative: a quiet environmental monitor is informative only if its sensitivity and coupling bound the disturbance needed to explain the candidate.

## ↑ Ancestors (6)

1. [GW150914](gw150914.md)
2. [Gravitational wave](gravitational-wave-split.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
