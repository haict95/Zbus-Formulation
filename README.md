# Zbus-Formulation

Most of zbus formulation programs that i found from the internet simply formulates the Ybus
then takes inverse of it to get Zbus, this approach is easier to do but when you to work
on a large system, things are gonna be much more complicated if you want to modify the networks or
do further analysis (fault, stability,..)

Basically, the system consists of busses, lines and power sources.

Algorithm:
1. Adding power source impedance to busses that have power sources.
2. Adding 1.0 impedance from busses that have no power sources to the ground.
3. Adding line impedances, each by each, from bus.. to bus..
4. Adding -1.0 impedance from busses that have no power sources to the ground.
