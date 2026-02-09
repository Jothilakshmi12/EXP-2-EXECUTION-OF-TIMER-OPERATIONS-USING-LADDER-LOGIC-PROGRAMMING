# EX02- EXECUTION OF TIMER OPERATIONS USING LADDER LOGIC PROGRAMMING.


 #### NAME : JOTHILAKSHMI PALANI
 #### REGISTER NUMBER : 212223110017
 #### DEPARTMENT: B.E.CSE(IOT)
 #### YEAR: III
 ### DATE: 03.02.2026

 
# Aim:
To understand and implement timer operations in a PLC using ladder logic and verify the output for different types of timers (ON-delay, OFF-delay, and Retentive timers).

# Apparatus Required:
Programmable Logic Controller (PLC) - A PLC that supports timer functions.
PLC Programming Software - Software such as RSLogix, TIA Portal, or CX-Programmer.
Computer System - For programming and simulating the PLC ladder logic.
Input Devices - Push buttons or switches for triggering the timer operations.
Output Devices - LEDs or any other indicators to visualize the timer output.
Wires and Connectors - For interfacing input/output devices with the PLC.
Power Supply - Appropriate power supply for the PLC and peripherals.
# Theory:
Timers in PLCs are used to introduce delays in control processes. They are fundamental in operations where the timing of events is crucial, 
such as starting a motor after a delay, turning off a light after a specified time, or maintaining a state for a fixed duration.

# Types of Timers:
 1. ON-Delay Timer (TON)
Functionality:

The ON-delay timer starts timing when the input condition becomes TRUE (ON).
After the preset time has elapsed, the timer output becomes TRUE (ON).
If the input condition turns FALSE (OFF) before the timer completes, the timer resets, and the output remains FALSE.

2. OFF-Delay Timer (TOF)
Functionality:

The OFF-delay timer starts timing when the input condition turns FALSE (OFF).
The timer output remains TRUE (ON) during the preset delay time and then turns FALSE (OFF) after the time has elapsed.
If the input condition becomes TRUE (ON) during the timing process, the timer resets.

3. Retentive ON-Delay Timer (RTO)
Functionality:

The Retentive ON-delay timer accumulates time as long as the input condition is TRUE (ON).
The accumulated time is retained even if the input condition turns FALSE (OFF).
The timer continues from the accumulated time when the input condition becomes TRUE again.
A separate reset input is usually provided to clear the accumulated time.

4. Pulse Timer (TP or TONR)
Functionality:

The Pulse Timer generates an output pulse of a specific duration when the input condition becomes TRUE (ON).
The output remains TRUE for the preset duration, regardless of the input state.

5. Timer-On Interval (TONI)
Functionality:

The Timer-On Interval is a variation of the ON-delay timer but is used to measure the time interval while the input is TRUE (ON).
The timer counts up as long as the input is TRUE and resets when the input turns FALSE.

 
# Procedure:
Setup the PLC Programming Environment:

Connect the PLC to the computer and launch the PLC programming software.
Ensure all input and output devices are connected to the PLC’s I/O modules.
Create Ladder Logic for Timers:

Implement the ON-delay timer (TON) by creating a rung with an input (e.g., a push button) linked to a TON instruction. Set the preset time (e.g., 5 seconds).
Implement the OFF-delay timer (TOF) by creating a rung with an input linked to a TOF instruction. Set the preset time (e.g., 5 seconds).
Implement the Retentive Timer (RTO) by creating a rung with an input linked to an RTO instruction. Set the preset time and enable an additional rung to reset the timer when required.
Simulate the Ladder Logic:

Run the simulation in the PLC software.
Test the ON-delay timer by pressing the input button and observing the delay before the output is activated.
Test the OFF-delay timer by deactivating the input and observing the delay before the output turns off.
Test the Retentive Timer by toggling the input on and off, observing how the accumulated time is retained.
Download and Execute:

Download the ladder logic program to the PLC if available and run it.
Test the timers with the physical push buttons and observe the LEDs or other output devices.

#   Outputs:
ON-Delay Timer: The output LED or indicator should turn on after a specified delay (e.g., 5 seconds) once the input is activated.
OFF-Delay Timer: The output should remain on for the specified delay after the input is deactivated, and then it should turn off.
Retentive Timer: The output should turn on after the accumulated time reaches the preset value, and it should retain the accumulated time even if the input is turned off.


# Simulation Screenshots 


<img width="818" height="318" alt="Screenshot 2026-02-03 112835" src="https://github.com/user-attachments/assets/c25e2901-6e87-4016-893f-4c382e7a5c11" />


<img width="660" height="217" alt="Screenshot 2026-02-03 112848" src="https://github.com/user-attachments/assets/3db8b6bf-acef-4009-95c6-3571980ccfb9" />


<img width="651" height="384" alt="Screenshot 2026-02-03 112859" src="https://github.com/user-attachments/assets/70ba75c3-1513-423f-9a24-1fcdf21e2f51" />


<img width="657" height="386" alt="Screenshot 2026-02-03 112909" src="https://github.com/user-attachments/assets/b173f434-77ae-40bc-b981-a271813ae101" />


<img width="668" height="374" alt="Screenshot 2026-02-03 113029" src="https://github.com/user-attachments/assets/4448b814-aa35-428e-b4d8-299548ac6a69" />


<img width="651" height="138" alt="Screenshot 2026-02-03 113043" src="https://github.com/user-attachments/assets/a425752f-2b2d-4e47-ac0f-edeb55a52740" />


<img width="736" height="383" alt="Screenshot 2026-02-03 113107" src="https://github.com/user-attachments/assets/02ffafc9-b0eb-4e8d-9216-d69be72c8a91" />


<img width="703" height="389" alt="Screenshot 2026-02-03 113118" src="https://github.com/user-attachments/assets/7f764462-f00a-4d13-8b3b-c7c339776c58" />


<img width="656" height="390" alt="Screenshot 2026-02-03 113127" src="https://github.com/user-attachments/assets/8bbd0f77-4aa5-4cf8-a9da-aea34e6382d5" />


<img width="684" height="307" alt="Screenshot 2026-02-03 113137" src="https://github.com/user-attachments/assets/d6ca76ff-eee5-4450-940f-d0fe0529db03" />


<img width="804" height="201" alt="Screenshot 2026-02-03 113505" src="https://github.com/user-attachments/assets/e35cac80-07f9-4cfc-a91d-71463e26b47e" />


<img width="1919" height="1079" alt="Screenshot 2026-02-03 112723" src="https://github.com/user-attachments/assets/54809bd3-5828-41ca-969b-90e847f6af2b" />



# Results:
The ladder logic programs for ON-delay, OFF-delay, and Retentive timers were successfully implemented and tested.
The observed outputs matched the expected behavior of each type of timer, demonstrating the correct functioning of timer operations in PLC ladder logic.
The experiment confirms the practical application of timers in controlling process sequences and managing time-dependent operations in industrial automation.
