# Electret Mic Preamp Build Notes 2/24/20
 
**Design Notes:**

This Electret Mic Preamp is a passive preamplifier and is based around the [LM358 op amp](https://www.ti.com/product/LM358).  This is a dual operational amplifier where in this circuit we are utilizing only one of the amplifiers on pins 1, 2, and 3.  Pin 4 is the Ground, where pin 8 is VCC.  
![](https://i.imgur.com/hkirKNo.png)
 
Pin 8 is powered by a 5v source, through two capacitors for filtering out high/low level noise (C2 and C3).  The electret mic is powered through a 10k resistor (R1), where the signal then goes through a coupling capacitor (C1) before a 1k resistor (R2) and entering pin 2.  A 200k variable resistor (VR1) serves to create feedback and the relationship between R2 and VR1 establishes the potential gain of the signal being represented by Gain = VR1/R2.  In this circuit, there is a potential gain of up to 200x the original signal (200k/1k = 200), allowing for a wide range of adjustment.

Two 100k resistors (R4/R5) are connected to GND and VCC respectively, prior to connecting to pin 3, for setting the potential voltage (2.5v). The circuit also has a power indicating LED for showing that the unit is powered on. 

# Build Process
**Bits:**
1/32” 
1/64”
**Mill Time:**
6m15s

It’s easiest to solder in this order:
```
1. Resistors
2. Ceramic Caps
3. Electret Mic
4. Dip Socket
5. LED
6. Electrolytic Caps
7. Screw Terminal 
8. Potentiometer
```
 

