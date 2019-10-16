LTspice output stage simulations
================================

This directory contains the LTspice source files used in the 
design phase of the Fastino output stage.

 - Design.asc: The proposed output stage design.
 - Design Monte-Carlo tolerance analysis.asc: A component
   tolerance analysis for the proposed design (mc() in LTspice
   uniformly samples from the given relative tolerance region).
 - Design with MFB second stage.asc: An alternative design
   providing enhanced high-frequency roll-off at the cost of an
   extra matched resistor pair and slightly increased noise and
   power dissipation.
 - Noise estimate using DAC matched Rs.asc: A quick estimate of
   the output noise from the DAC-internal matched resistor pair.
 - Stabilizer output stage design.asc: For comparison, the
   output stage of the Stabilizer v1.0 two-channel
   microcontroller servo.

The macromodels for the OPA197 and AD8620 can be downloaded from
the respective manufacturer's websites; place them somewhere on
the library search path (in the easiest case, this directory):

 - http://www.ti.com/product/OPA197/toolssoftware
   (the PSpice model can be used with LTSpice)
 - https://www.analog.com/media/en/simulation-models/spice-models/ad8620.cir
