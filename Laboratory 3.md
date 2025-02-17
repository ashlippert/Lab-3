# Lab 3: Let's Switch

**Authors:**

Ashlyn Lippert and Seth Daniel

**Date:**

February 17th, 2025

## Introduction
   Transistors are essential in modern electronics, with Bipolar Junction Transistors commonly used for amplification and switching. This lab focuses on understanding BJTs by using the TIP 31C transistor as a switch to control current through an LED and a motor. We will explore its different operating modes and how factors like gain (β) affect performance.

   Additionally, we will examine diodes, which allow current to flow in one direction, and LEDs, which emit light when current passes through them. This lab provides hands-on experience with semiconductor devices and their applications in circuit design.

## Materials
1. Resistors: 1kΩ, 2.2 Ω, 270 Ω, 1 kΩ
2. DC Power Supply (DCPS)
3. Fluke 87 V DMM
4. A NTE 125 Diode
5. Additional wires
6. A designated "switch" wire
7. An electric motor (from the Sparkfun inventor's kit)
8. A 1kΩ trimmer potentiometer
9. A TIP31C transistor
10. A LED
11. Flathead screwdriver

## Assembly Methods

**Objective: Learn to use Diodes, LEDs, and transistors in a basic circuit**

1. **LED Directly Connected to a Switch**

   The circuit was constructed according to the schematic in Figure 1. Voltages were measured at each test point with respect to ground, ensuring accurate readings by placing the multimeter’s black probe close to the switch terminal. Ohm’s Law was used to calculate the currents through the resistor (R1), using only components with known resistance. For this circuit, the sliding switch was replaced by a wire, where when one end was disconnected the switch was "OFF" and with both ends connected the switch is "ON".

<div align= "center">
<img src="https://github.com/user-attachments/assets/ae1d075f-1e65-430c-be60-8a4bf0e01eb2" alt "Schematic 1" width="200"/>
<br>
<figcaption style="font-size: 16px; text-align: center;"> Figure 1: Schematic describing the LED switch circuit built for part 1 of this lab. </figcaption>
</div>

<br>

   The circuit created using this schematic should resemble what is shown in Figure 2 below.

<div align= "center">
<img src="https://github.com/user-attachments/assets/c80a1233-a255-454c-b93a-becd8e07ac8d" alt "Circuit 1" width="400"/>
<br>
<figcaption style="font-size: 16px; text-align: center;"> Figure 2: Constructed circuit from Schematic 1. </figcaption>
</div>

<br>

2. **LED Driven by a Transistor**

   A new circuit was built to drive the LED using a transistor in the schematic shown in Figure 3. Voltages were measured at all test points, and currents were calculated using known resistor values. The current through the LED was compared to that of the previous circuit to analyze differences.  

   Additionally, the transistor’s voltage drop was recorded and compared with the calculated expected values. The power supply was adjusted to observe changes in IC to help determine whether the transistor operated in the saturation region. The schematic for constructing this circuit is shown in Figure 3. The wire switch was also used for this circuit in place of a sliding switch.


<div align="center">
<img src="https://github.com/user-attachments/assets/66f77f2e-4f49-4d3a-93f6-4861215dcae8" alt="Schematic 2" width="400"/>
   
<br/>
   
  <figcaption style="font-size: 16px; text-align: center;"> Figure 3: LED driven by transistor with a fixed current schematic. </figcaption>
</div>

<br>

   When constructed, the circuit assembled using Schematic 2 should resemble Figure 4.

   <div align="center">
  <img src="https://github.com/user-attachments/assets/dd238a1d-5742-4368-ac3d-01adf5b8a011" alt="Circuit 2" width="400"/>
      
<br>

   
  <figcaption style="font-size: 16px; text-align: center;"> Figure 4: Constructed circuit from Schematic 2. </figcaption>
</div>   


<br>

3. **LED Current Controlled Using a Transistor**

   A potentiometer is introduced to control the base current of the transistor, effectively modulating the LED brightness. By adjusting the resistance, the base current changes, influencing the collector current and thus the LED’s brightness. This circuit demonstrates how transistors can be used for more than just on-off switching, they can also provide variable control.

   The schematic for constructing this circuit is provided in Figure 5 below.


<div align="center">
<img src="https://github.com/user-attachments/assets/5ecb04b3-15b5-48c6-80de-66bd0e2c849e" alt="Schematic 3" width="400"/>
<br/>
  <figcaption style="font-size: 16px; text-align: center;"> Figure 5: Controlling LED current using a transistor schematic. </figcaption>
</div>


<br>


   When constructed, the circuit assembled using Schematic 3 should resemble Figure 6.
   
<br>

<div align="center">
<img src="https://github.com/user-attachments/assets/bb907543-c792-47d3-a7fe-ccaed9e8d0af" alt="Circuit 3" width="400"/>
      
<br>

  <figcaption style="font-size: 16px; text-align: center;"> Figure 6: Constructed circuit from Schematic 3. </figcaption>
</div>   


<br>


**Objective 2: Motor Driven Circuit**


1. **Motor Speed Control Using a Transistor**

   In this circuit, a transistor is used to control the speed of a DC motor. Similar to the LED circuit, the transistor acts as a switch, allowing current to flow when the base is activated. A potentiometer is used to modulate the base current, thereby adjusting the motor’s speed. The diode is placed in parallel with the motor to protect against voltage spikes caused by inductive loads.
   Schematic 4 shown below describes the construction for the transistor controlled motor circuit.


<div align="center">
<img src="https://github.com/user-attachments/assets/db1927d1-b8ee-47f9-a5d6-02810c6a91e9" alt="Schematic 4" width="400">
<br/>

<figcaption style="font-size: 16px; text-align: center;"> Figure 7: Transistor controlled motor current and speed schematic. </figcaption>
</div>   

<br/>
  Once assembled, the circuit should look resemble Figure 8 below.

   <div align="center">
  <img src="https://github.com/user-attachments/assets/d2981ce5-c15f-4577-a524-8122d3324fc7" alt="Assembled parallel resistor circuit" width="400">
      <br/>
  <figcaption style="font-size: 16px; text-align: center;"> Figure 7: Transistor controlled motor current and speed schematic. </figcaption>
</div>


<br>

## Test Equipment

1. Fluke 87 V DMM
2. DC Power Supply
   
## Test Procedures

**Resistor Measurement**

   For this part of the experiment, the resistance each resistor was measured using a Digital Multimeter (DMM) and the results were compared to the expected values based on the resistor color codes. We recorded the expected resistance, the acceptable tolerance range, and the measured resistance in a table. Any resistors that fell outside the expected range were noted.

**Part 1.1: LED Directly Connected by a Switch**

1. **Voltage and Current Measurements:**
   
   Using the circuit created in objective 1.1 of the assembly procedures, connect the terminal of R1 and the switch to the DC Power Supply using the alligator clips. Ensure black is connected to - terminal (ground) and red is connected to the + terminal.
   Once connected, set the DCPS to 5 V and press the OUTPUT ON button to begin delivering power to the circuit. Next, using the DMM, measure the voltage at each point with respect to ground (T4) and record the results in a table. Attach the black (COMMON) multimeter probe to a point close to the switch terminal. Be sure to record each voltage for the switch ON and the switch OFF.
   Try to measure as close to the resistor terminal as possible to avoid any small voltage drops. Additionally, measure the voltage across each component in the circuit (R1, LED, switch) and record in the table. See Figure 9 for how voltage across each component was measured. Use the measured voltages to calculate the currents through each resistor.
   Change the DMM settings and lead connections to measure current, then record the current through the LED in the circuit for the switch ON and OFF.

<div align="center">
  <img src="https://github.com/user-attachments/assets/ee69acd4-0dfe-4854-847b-8f4fff4db869" alt="Measuring Voltage Across" width="400">
      <br/>
  <figcaption style="font-size: 16px; text-align: center;"> Figure 9: Measuring voltage across a resistor using the DMM. </figcaption>
</div>


**Part 1.2: LED Driven by a Transistor Circuit**

1. **Voltage and Current Measurements:**
 
  Using the circuit created in objective 1.2 of the assembly procedures, connect the point T7 to the 5VDC output and T1 to the main output using the alligator clips.
   Once connected, set the DCPS to 5 V and press the OUTPUT ON button to begin delivering power to the circuit. Next, using the DMM, measure the voltage at each point with respect to ground (T4) and record the results in a table. Make sure to record each voltage for the switch ON and the switch OFF. Try to measure as close to the resistor terminal as possible to avoid any small voltage drops.
   Also measure the voltage across each component in the circuit, such as R1, LED, R2, and the switch and record in the table. Use the voltages to calculate the currents through the various resistors.
   Change the DMM settings and lead connections to measure current, then record the current through the LED and R2 in the circuit for the switch ON and OFF.


<div/>
   
**Part 1.3: Controlling LED Current Using a Transistor Circuit**

   1. **Voltage and Current Measurements:**
  Using the circuit created in objective 1.3 of the assembly procedures, connect R3 and T1 to the 5VDC output and the other end of R3 and T4 to ground using the alligator clips.
   Once connected, set the DCPS to 5 V and press the OUTPUT ON button to begin delivering power to the circuit. Next, using the DMM connected to T2, measure the voltage while adjusting the 1 kΩ potentiometer. Once the voltage at T2 is not changing, you can declare your minimum and maximum LED brightnesses. Additionally, identify two intermediate (midpoint) voltges between the dim and bright LED settings. The method used for adjusting the potentiometer is shown in Figure 10 below.

<div align="center">
  <img src="https://github.com/user-attachments/assets/ff4316f2-4f2a-442a-a28a-cd46efaa3b5c" alt="Measuring Voltage Across" width="400">
      <br/>
  <figcaption style="font-size: 16px; text-align: center;"> Figure 10: Adjusting the potentiometer voltage output. </figcaption>
</div>

   For each potentiometer setting, measure the voltage at each test point and the voltage across each component (R1, LED, R2). Try to measure as close to the resistor terminal as possible to avoid any small voltage drops. Record all values in the table.
   Change the DMM settings and lead connections to measure current, then record the current through the LED and R2 in the circuit for each potentiometer setting. Using the LED current (Ic) and the R2 current (Ib), calculate the gain.
   

**Part 2.1: Controlling Motor Current and Speed Using a Transistor**

   Use the circuit assembly from of objective 2.1 of the assembly procedures. Once assembled, use ta screwdriver too adjust the voltage level of the 1kΩ potentiometer. Connect the DMM to T2, and if the voltage is not changing identify these points as the minimum and maximum speed of the motor. Additionally, choose two intermediate voltages (midpoints) between the minimum and maximum motor speed.
   For each potentiometer setting, measure the voltage at each test point and the voltage across each component (R1, M1, R2). Try to measure as close to the resistor terminal as possible to avoid any small voltage drops. Record all values in the table.
   Change the DMM settings and lead connections to measure current, then record the current through the M1 and R2 in the circuit for each potentiometer setting. Using the motor current (Ic) and the R2 current (Ib), calculate the gain.
   
## Test Results:

**Table 1: Resistor Values**

| Resistor # | Expected Resistance (Ohms) | Tolerance | Max Value (Ohms) | Min Value (Ohms) | Measured Resistance (Ohms) |
|------------|----------------------------|-----------|------------------|------------------|----------------------------|
| 1          | 2.2                        | 5%        | 2.31             | 2.09             | 2.24                        |
| 2          | 270                        | 5%        | 283.5            | 256.5            | 268.9                       |
| 3          | 1000                       | 5%        | 1050             | 950              | 984                         |

**Table 2: DCPS Voltage Verification**
| Expected DCPS Voltage Output (V) | Measured Voltage with DMM (V) |
|----------------------------------|-------------------------------|
| 5                                | 5.01                          |

**Table 3: LED Directly Controlled by a Switch**

| Test Point |     Voltage (Switch On)     |     Voltage (Switch Off)     |
|------------|-----------------------------|------------------------------|
| T2         | 2.045 V                     | 0.163 V                      |
| T3         | 0 V                         | 0  V                         |

| Component  |  Voltage Across (Switch On) |  Voltage Across (Switch Off) |
|------------|-----------------------------|------------------------------|
| R1         | 2.95 V                      | 0 V                          |
| LED1       | 2.05 V                      | 0.171 V                      |
| S1         | 0 V                         | 0 V                          |

|            | Current Through (Switch On) | Current Through (Switch Off) |
|------------|-----------------------------|------------------------------|
| LED1       | 0.012 A                     | 0 A                          |

**Table 4: LED Controlled by a Transistor**

| Test Point |     Voltage (Switch On)    |     Voltage (Switch Off)      |
|------------|----------------------------|-------------------------------|
| T2         | 2.047 V                    | 5.003 V                       |
| T3 (VCE)   | 0.013 V                    | 3.518 V                       |
| T5 (VBE)   | 0.682 V                    | 0.170 V                       |
| T6         | 5 V                        | 0.135 V                       |

| Component  | Voltage Across (Switch On) |  Voltage Across (Switch Off)  |
|------------|----------------------------|-------------------------------|
| R1         | 2.914 V                    | 0 V                           |
| LED1       | 2.045 V                    | 0.390 V                       |
| R2         | 4.4 V                      | 0 V                           |
| S1         | 0 V                        | 0 V                           |

|            | Current Through (Switch On) | Current Through (Switch Off) |
|------------|-----------------------------|------------------------------|
| LED1 (IC)  | 0.012 A                     | 0 A                          |
| R2 (IB)    | 0.005 A                     | 0 A                          |


**Table 5: Adjusting LED Brightness with a Transistor**

|  Test Point |     Dim LED Voltage    |     Midpoint 1 Voltage    |     Midpoint 2 Voltage    |     Bright LED Voltage    |
|-------------|------------------------|---------------------------|---------------------------|---------------------------|
| T2          | 4.97 V                 | 4.86 V                    | 2.62 V                    | 2.057 V                   |
| T3 (VCE)    | 3.26 V                 | 3.063 V                   | 0.530 V                   | 0.011 V                   |
| T5 (VBE)    | 0.459 V                | 0.515 V                   | 0.592 V                   | 0.683 V                   |
| T6          | 0.459 V                | 0.518 V                   | 0.625 V                   | 4.992 V                   |

|  Component  | Voltage Across Dim LED | Voltage Across Midpoint 1 | Voltage Across Midpoint 2 | Voltage Across Bright LED |
|-------------|------------------------|---------------------------|---------------------------|---------------------------|
| R1          | 0.015 V                | 0.130 V                   | 2.46 V                    | 2.94 V                    |
| LED 1       | 1.709 V                | 1.804 V                   | 2.015 V                   | 2.041 V                   |
| R2          | 0 V                    | 0.002 V                   | 0.033 V                   | 4.309 V                   |

|             | Current Through Dim LED| Current Through Midpoint 1| Current Through Midpoint 2| Current Through Bright LED|
|-------------|------------------------|---------------------------|---------------------------|---------------------------|
| LED (IC)    | 0.00007 A              | 0.00045 A                 | 0.00901 A                 | 0.01077 A                 |
| R2 (IB)     | 0.00001 A              | 0.00001 A                 | 0.00004 A                 | 0.00505 A                 |
| Gain (IC/IB)| 7                      | 45                        | 225.25                    | 2.132                     |

**Table 6: Motor Speed Control Using a Transistor**

|  Test Point |     Slow Motor Voltage    |     Midpoint 1 Voltage    |     Midpoint 2 Voltage    |     Fast Motor Voltage    |
|-------------|---------------------------|---------------------------|---------------------------|---------------------------|
| T2          | 4.825 V                   | 4.77 V                    | 4.74 V                    | 4.710 V                   |
| T3 (VCE)    | 2.917 V                   | 1.25 V                    | 0.476 V                   | 0.125 V                   |
| T5 (VBE)    | 0.633 V                   | 0.654 V                   | 0.669 V                   | 0.713 V                   |
| T6          | 0.847 V                   | 0.925 V                   | 1.0 V                     | 4.960 V                   |

|  Component  | Voltage Across Slow Motor | Voltage Across Midpoint 1 | Voltage Across Midpoint 2 | Voltage Across Fast Motor |
|-------------|---------------------------|---------------------------|---------------------------|---------------------------|
| R1          | 0.160 V                   | 0.198 V                   | 0.215 V                   | 0.238 V                   |
| M1          | 2.16 V                    | 3.459 V                   | 3.553 V                   | 4.6 V                     |
| R2          | 0.215 V                   | 0.274 V                   | 0.270 V                   | 4.25 V                    |

|             | Current Through Slow Motor| Current Through Midpoint 1| Current Through Midpoint 2| Current Through Fast Motor|
|-------------|---------------------------|---------------------------|---------------------------|---------------------------|
| M1 (IC)     | 0.0642 A                  | 0.0815 A                  | 0.10001 A                 | 0.108 A                   |
| R2 (IB)     | 0.00019 A                 | 0.00029 A                 | 0.00048 A                 | 0.00433 A                 |
| Gain (IC/IB)| 337.894                   | 281.034                   | 208.354                   | 24.942                    |

## Discussion:

Seth

## Conclusion:

This lab reinforced our understanding of circuit analysis by applying Kirchhoff’s laws, Ohm’s law, and Thevenin’s theorem. We built and tested series and parallel circuits, taking voltage and current measurements to compare with theoretical values. While most results aligned with expectations, some discrepancies were likely due to measurement errors or resistor tolerances. Additionally, soldering the series circuit provided valuable hands-on experience. Overall, the lab improved both our analytical and practical skills in circuit design and testing.

