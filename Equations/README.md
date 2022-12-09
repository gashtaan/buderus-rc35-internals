# Power and flow temperature targets calculation
RC35 continuously calculates target power and target flow temperature according to selected control mode. It's up to boiler to deliver these targets to the heating system.

## Outside temperature control mode
Target power:
$$P = 100$$
Target flow temperature:
$$T = T_r + 7a + (T_s - 27)b$$
$$a = \frac{ T_r - T_o }{ 20 - T_m }$$
$$b = a(C\frac { 1.0 - a } { 0.2 + a } + 1)$$

T<sub>r</sub> : room temperature target with offset and influence applied

T<sub>m</sub> : minimal outside temperature in region

T<sub>s</sub> : standard flow temperature at minimal outside temperature

T<sub>o</sub> : actual outside temperature

C : heating system coefficient (floor : 0.075, convector : 0.3, other : 0.2475)
