# Power and flow temperature targets calculation
RC35 continuously calculates target power and target flow temperature according to selected control mode. It's up to boiler to deliver these targets to the heating system.

## Outside temperature control mode
Target power:
$$P = 100$$
Target flow temperature:
$$T = 7a + (T_s - 27)b$$
Heating characteristic curve linear component:
$$a = \frac{ T_r - T_o }{ 20 - T_m }$$
Heating characteristic curve non-linear component:
$$b = a(c\frac { 1.0 - a } { 0.2 + a } + 1)$$
System coeficient:
$$c = \text { floor : 0.075, convector : 0.3, other : 0.2475 }$$
