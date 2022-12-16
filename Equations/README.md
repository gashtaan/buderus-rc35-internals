# Room temperature influence
If outside temperatuer control mode is selected and room temperature influence is set by user, RC35 virtually increase/decrease target room temperature. The greater the difference between target room temperature and actual room temperature is, the greater is level of increase/decrease. The infuence configured by user limits that change to some interval. Such affected room temperature target is then input to power and flow temperature targets calculation.
$$T_r = T_r + C$$
$$C = max(-I, min(F(T_r - T_a), 3I))$$

T<sub>r</sub> : target room temperature

T<sub>a</sub> : actual room temperature

I : room influence

F : multiplication factor defined in 5th parameter of HC parameter table (default 40 = 4.0)

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
