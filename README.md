#  Bi directional Voltage Source Inverter with PV array Grid connected and Off Grid Variants. 

Regulated by PWM and configured to american/European standard

![image](https://user-images.githubusercontent.com/89353805/130367878-7986d78b-58a0-4ed4-b5c3-c91bda2dbea7.png)

## Design Overview
The design of the inverter supports two modes of operation: a closed loop
single phase mode using an LC filter at the output and a resistor to simulate the load. The other mode of
operation is a grid-connected mode using an LCL filter at the output and a voltage source to simulate the
grid. The single phase mode is suitable for uninterrupted power supplies, while the grid-connected mode
is more suitable for photovoltaic applications such as solar panels. These modes of operation were
simulated within Simulink and MATLAB and later developed further using the Texas Instruments
inverter kit.

## Barebones Explanation
Closed loop mode essentially means that the inverter runs off grid. It is not connected to the main
regional power grid and fully sources its energy from solar radiation. Generated surplus or a shortage are
not usually rectifiable due to its independent nature. Pros being the ability to run on an independent
voltage and frequency while it cannot source some dependence from the main power line.
Grid Connected inverter is connected to the main electric grid. In the event of a surplus, it can transfer
the energy to the local grid and earn credits from the electric agency, whereas in the event of a shortage
it can request energy from the grid. Pros being it can never run out of power, while the downside is to
have the reference voltage matching the grid.

## Innovation in Testing

With the PV equipment in place, a constant 1000 level irradiance was attached to the panel. This didn't account for the variable sunlight and
radiation levels. To attempt to simulate more realistic conditions, a repeated sequence generator was
added into the design, to mimic variable sunlight (such as cloudy conditions, changing of the seasons,
etc.)


![image](https://user-images.githubusercontent.com/89353805/130368006-27811ea8-39fb-46d9-b089-9c325dddf979.png)


Implementation and working explained here: https://www.youtube.com/watch?v=yNYgXOfM-Xw

