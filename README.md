#  Bi directional Voltage Source Inverter with PV array Grid connected and Off Grid Variants. 

Regulated by PWM and configured to american/European standard

The design of the inverter supports two modes of operation: a closed loop
single phase mode using an LC filter at the output and a resistor to simulate the load. The other mode of
operation is a grid-connected mode using an LCL filter at the output and a voltage source to simulate the
grid. The single phase mode is suitable for uninterrupted power supplies, while the grid-connected mode
is more suitable for photovoltaic applications such as solar panels. These modes of operation were
simulated within Simulink and MATLAB and later developed further using the Texas Instruments
inverter kit.


https://github.com/arshv06/BidirectionalInverter/blob/6cbbdc81876a38a3b2370264cc615b0098191a37/Inverter-Final/Grid%20Connected/Inverter%20PV%20Schematic%20with%20variable%20Irradiation.png
Implementation and working explained here: https://www.youtube.com/watch?v=yNYgXOfM-Xw

