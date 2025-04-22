# Eurocard LNA v1
CONTEXT: v1 is still considered a work-in-progress, and I designed it to compensate my lack of a proper oscilloscope, so I took the occasion to try and learn something instead of spending some hundreds of €€€ on a scope (which is the logical way, but from which I don't actually learn anything). Since performances are deemed as acceptable for my everyday hobbyist use (at least for now) and since I like the idea of fitting it on an Eurocard PCB I thought I might work on such a design. Also, please remember that there is no need in building this whenever professional instruments are available.<br/>
Aka: I lack professional testing since I don't have the proper instruments to do so, and if I had them I would not need this design. Hence, my personal use is to build it and use it as a preamplifier for my USB oscilloscope.<br/>
DISCLAIMER: HP filters and selectable Sallen-key LP filters may need some adjustments, as some general adjustments here and there.

DESCRIPTION
A 1 Hz - 1MHz AC/DC battery powered, portable low noise preamplifier meant to be built on a Eurocard PCB (100x160 mm) and meant to be used for general purpose amplification (as an additional help for particularly noisy oscilloscopes/lack of proper ones). It is based upon four JFE2140 differential JFETs working in parallel to reduce V-noise, with gain set via non-inverting op-amps in two stages, giving selectable x100 and x1000 V-amplification.

CURRENT CAPABILITIES:
- Battery operated (four 14500 Li-ion batteries).
- Selectable AC/DC operation.
- IN/OUT connection via 50 Ohm BNCs.
- Amplification down to around 50 microV (according to theoretical calculations and simulations) in full bandwidth mode (i.e. highest wideband noise).
- Optional LP filters to reduce BW (around 200 Hz/20k Hz -the second good for audio purposes-, selectable).
- SMD formats chosen to be as far as possible compatible with hand-soldering (R and C are mostly 1206 format -with very few exceptions, which are 0603-, ICs are SOIC, transistors are SOT).
