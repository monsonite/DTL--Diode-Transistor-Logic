# DTL--Diode-Transistor-Logic


A menagerie of logic building blocks simulated in DTL, so that they may be built using discrete components.

DTL is the forerunner of TTL. It was first produced in the 1950s using discrete transistors and moved across to integrated form (in DIL packages) in the early 1960s.

DTL is characterised as being a transistor inverter, with the gate being pulled low through multiple input diodes. The result is a NAND gate.

A generic DTL 2-input NAND gate is shown below (Wikipedia):

![image](https://github.com/monsonite/DTL--Diode-Transistor-Logic/assets/758847/b0931fb3-14c5-47f7-8ae9-a6e17ffd487e)

Pull down resistor R4 is often omitted, and R3 is often replaced with 2 diodes, forwards biassed by current flowing down R1. The 2 diodes in series provides a voltage "hurdle" of approximately 1.3V, which means that the voltage offset between logic low and logic high is Vbe +1.3V, which greatly improves noise immunity.

In a fairly recent development by Tim Boscke, R3 has satisfactorily replaced with a red or green LED, which not only provides a suitable forward voltage drop, but illuminates to indicate when the tranistor is in the saturated on state.  Tim Boscke has produced a simple CPU using the LED-Transistor Logic - and this article describes the logic and its characteristics in detail.

Here is the basic LTL 2 input NAND gate.

![image](https://github.com/monsonite/DTL--Diode-Transistor-Logic/assets/758847/81eec45b-9ad9-4336-9444-477c86ca3053)

And this is the LTL AND-OR-INVERT - useful for making XOR gates for ALUs and multiplexers

![image](https://github.com/monsonite/DTL--Diode-Transistor-Logic/assets/758847/f7d2e73f-a4db-4697-8677-5ea4cc850d07)

Here is the XOR gate made from an A-O-I gate and two inverters

![image](https://github.com/monsonite/DTL--Diode-Transistor-Logic/assets/758847/8b9edc17-9302-4ce7-9f99-c42a37363642)



https://hackaday.io/project/169948-lcpu-a-cpu-in-led-transistor-logic-ltl

DTL (or LTL) is a popular choice for discrete transistor based logic mainly because of its low component count and robust characteristics. It is well suited to implementation using surface mount components, if a greated logic density or the precision of a machine build is required.

Using through-hole components, a 3-input LTL NAND occupies 12x12mm of pcb area.




