# Energia-IDE
1. Joystick to Seven-Segment Display
   
This project utilizes the MSP432P4111 LaunchPad and a joystick to control a seven-segment display simulated on an LCD screen. The joystick's Y-axis movement is read using the ADC (Analog-to-Digital Converter), and its value is mapped to a range of 0 to 99. The mapped value is then displayed on the LCD screen, mimicking a two-digit seven-segment display. The project is programmed using Energia IDE, leveraging its built-in libraries for LCD control and analog input handling. The default display value starts at 46, and as the joystick is moved along the Y-axis, the values change accordingly—showing 00 at one extreme and 99 at the other, with intermediate values in between. This experiment demonstrates ADC signal processing, real-time display updates, and embedded UI design, providing hands-on experience with sensor integration and data visualization on microcontrollers.



2. Joystick for Accelerometer
   
This project involves interfacing a 3-axis accelerometer (Kionix KXTC9-2050) with the MSP432P4111 LaunchPad to measure and display real-time acceleration values along the X, Y, and Z axes. The accelerometer detects motion and tilt, generating signals that correspond to acceleration due to movement and gravity. Using Energia IDE, the analog acceleration values are read and displayed on an LCD screen. Additionally, a MATLAB program is used to visualize the acceleration data in real-time by plotting the values on a 3D graph. A delay is introduced between readings to ensure accurate plotting. By tilting the board in different directions, changes in X, Y, and Z-axis acceleration can be observed both on the LCD and MATLAB plot. This project demonstrates sensor integration, real-time data acquisition, serial communication, and graphical representation, providing practical experience in embedded systems and motion sensing applications.


3. Timer and PWM Generation
   
This project focuses on Pulse Width Modulation (PWM) signal generation using the MSP432P4111 LaunchPad and its built-in Timer_A module. The goal is to generate a 10Hz square wave with a 50% duty cycle and observe its behavior under different timer output modes and counting modes. Using Energia IDE, the Timer_A0 is configured to generate PWM signals on specific output ports (P2.4, P2.5, P2.6, and P2.7). The project explores three timer output modes—Toggle/Reset (Mode 2), Toggle (Mode 4), and Reset/Set (Mode 7)—under two different counting modes: Up mode and Up/Down mode. The ACLK (32.768 kHz clock) is used to determine the correct TACCR0 and TACCR1 values for the desired PWM frequency.By modifying the timer settings, different waveform behaviors are observed, allowing for precise control of duty cycles and output signals. This experiment provides hands-on experience in timers, PWM signal generation, frequency calculation, and embedded system timing control, which are essential for motor control, LED dimming, and communication protocols.


4. Energy Efficiency Calculation
   
This project evaluates the power consumption of the MSP432P4111 LaunchPad in Active Mode versus Low Power Mode 3 (LPM3) to understand energy efficiency in embedded systems. The MSP432 operates in two states:

Active Mode: The CPU executes instructions while continuously toggling a Blue LED.

Low Power Mode 3 (LPM3): The CPU is halted, with only essential peripherals running, indicated by a Green LED.

Using Energia IDE, the system monitors current consumption via a current sensor on the Booster Pack. Power consumption is calculated using P = V × I, and energy usage is determined as E = P × time. These values are displayed on the serial monitor when switching between modes via a push button. This experiment demonstrates low-power design techniques, showcasing how microcontrollers optimize power consumption for energy-efficient applications. It is crucial for battery-powered devices, IoT systems, and real-time embedded applications that require efficient power management.
