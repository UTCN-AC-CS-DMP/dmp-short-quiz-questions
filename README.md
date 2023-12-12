# DMP SHORT QUIZ QUESTIONS

<details>
<summary>Lab 1 - click to expand / close</summary>

## Lab 1

### Questions from LECTURE 1 documentation

1. What is a Central Processing Unit?
2. What is a microprocessor?
3. What is a microcontroller?
4. Describe the term "computer program"
5. What are the four steps as to how instructions are usually executed? (Think back to the MIPS from last year)
6. What is the term that defines as to what instructions the microprocessor / microcontroller supports? (Answer: ISA - Instruction Set Architecture)
7. What family of microcontrollers does the Arduino MEGA 2560 development board use?
8. In terms of the SUPPORTED INSTRUCTIONS, what is the architecture of the microcontroller used by the Arduino MEGA? (RISC or CISC)
9. What is the difference between CISC and RISC architecture?
10. In terms of the STORAGE AND PATHWAYS FOR INSTRUCTION AND PROGRAM MEMORY, what is the architecture of the microcontroller used by the Arduino MEGA? (Harvard or Von Neumann)
11. What is the difference between H & VN?
12. What are the individual parts of the two-stage pipeline of the AVR? (Answer: Fetch & Execute)
13. How many General Purpose Registers (GPS) are there in the AVR?
14. Within which registers can you load immediate values? (Answer: R16-R31)
15. What are the DATA COPY register operations supported by the AVR?
16. What are the IMMEDIATE register operations supported by the AVR?
17. What are the ALU based register operations supported by the AVR?
18. What type of memory is used for the Program Memory? (Answer: flash)
19. What 8-bit register contains information about the state of the microcontroller and about the result of operations?

### Questions from LABORATORY 1 documentation

1. What kind of MCU does the Arduino MEGA 2560 board use and on how many bits does it operate on?
2. What are some of the communication protocols / interfaces (facilities) that the development board supports? (Answer: UART, SPI, I2C)
3. What is the speed (operating frequency) of the MCU? (Answer: 16 MHz)
4. Explain the difference between pull-up and pull-down resistors
5. What is the name of the defined flag that activates the internal resistors of the development board? (Answer: INPUT_PULLUP)
6. Why is a breadboard useful? (Any answer can be given, but one advantage is that the pins can be electronically connected to the same source)
7. What is the parameter of the Serial.begin(VALUE) method?
8. What is the method to set a certain pin on the dev board as input / output / input_pullup?
9. What is one method that you can use in order to get a value from a certain pin?
10. Explain the '<<' operator from C / C++
11. Give an example of how to find out as to how long your Arduino based application has been running in SECONDS
</details>

<details>
<summary>Lab 2 - click to expand / close</summary>


## Lab 2

### Questions from LECTURE 2 documentation

1. What are the Input / Output ports for the Arudino Mega? 
(Answer: A B C D E F G H J K L, the letter I is missing on purpose, source: https://github.com/arduino/ArduinoCore-avr/blob/master/variants/mega/pins_arduino.h
2. What register would you use to configure a certain port as either input or output?
3. What register would you use to write to a certain port?
4. What register would you get a certain port's state?
Additional info for questions 2-4 https://forum.arduino.cc/t/relationship-among-portx-pinx-ddrx-pinmode-of-arduino/457412

### Questions from LABORATORY 2 documentation

1. How would you configure all the pins of port A as input?  (Answer: DDRA = 0b00000000;)
2. How would you configure all the pins of port A as output? (Answer: DDRA = 0b11111111;)
3. How would you configure the lower half of port B as output and the upper half of it as input? (Answer: DDRB = 0b00001111;)
4. How would you read data from port A? (Answer: set all pins as input, then assign value to a variable: DDRA = 0; char a = PINA)
5. Give an example of transmitting data from port A of the MCU to a peripheral (Answer: 8 LEDs are hooked up to the port and to make half of them light up: DDRA = 0xFF; PORTA = 0b10101010;)
6. What does the C / C++ macro "<variable_name> = <condition> ? <val1> : <val2>" do?
7. What is the operator for the "BITWISE or" operation in the C / C++ programming language?
8. What is the operator for the "BITWISE XOR" operation in the C / C++ programming language?
9. Explain the following line of code: "cdigit ^= 1;" (Same as "cdigit = cdigit ^ 1;")
10. Explain the terms LSB and MSB, what does the acronym stand for and what is the meaning behind it
</details>

<details>
<summary>Lab 3 - click to expand / close</summary>

## Lab 3

### Questions from LECTURE 3 documentation

1. What is the general term for a function that gets executed when an interrupt is triggered?
2. How many different triggering modes are there and explain them
3. What attribute do you have to give to a global variable if you plan to use them inside an ISR? Why?
4. How many ISR functions can run at the same time?
5. Should you use the delay(), millis(), micros() methods inside an ISR? What's something similar that you can use?
6. Is it recommended to use the Serial interface in an ISR?

### Questions from LAB 3 documentation

1. When it comes to electronics, what does the acronym PCB stand for?
2. When using a third-party shield with a development board, what is something that needs to be taken into consideration regarding the pins?
3. What is the LCD controller used during the labs?
4. When generating characters to be displayed on the LCD, what specifies which pixel will be turned on or off?
5. What header file do you have to include in your source code in order to use the LCD?
6. How do you set the number of rows and columns to be used with the LCD?
7. What method can you use in order to load a user-defined custom character into the CGROM?
8. What method would you use to display a custom character and what kind of variable type does it need as the parameter?
9. In order to trigger interrupts, what two bits have to be enabled in an Arduino system?
10. What assembly instruction does every ISR end with implicitely? Why?
11. Explain the difference between the two types (internal & external) of interrupts
12. What stores the addresses of the ISRs?
</details>

<details>
<summary>Lab 4 - click to expand / close</summary>

## Lab 4

### Questions from LECTURE 4 documentation

1. Name three basic usages for external HW timers
2. Which register controls a timer's working mode?
3. How do you configure a timer's speed (frequency)?
4. Which flag can be used for generating an interrupt for the CPU?
5. Which two registers would you use for generating waveforms?
6. What is the difference between normal and CTC modes?
7. What is the difference between fast PWM and phase correct PWM?

### Questions from LAB 4 documentation

1. What is the TCCRx register and what is it used for?
2. What is the TCNTx register and what is it used for?
3. What is the OCRx register and what is it used for?
4. What is the ICRx register and what is it used for?
5. What is the TIMSKx register and what is it used for?
6. What is the TIFRx register and what is it used for?
7. What function / method do you use for tone generation, what are the parameters?
8. What function / method can you use for generating a PWM signal, what are the parameters?
</details>

<details>
<summary>Lab 5 - click to expand / close</summary>

## Lab 5

### Questions from LECTURE 7 (NOT 5!!!) documentation
1. What are the two signals (wires) that are used for I<sup>2</sup>C communication?
2. What are the two signals (wires) that are used for UART communication?
3. How do you connect two devices that use UART communication?
4. How do you check if data is available in the UART interface's buffer?
5. Which user defined function is called automatically when data is available in the UART interface's buffer?
6. What library do you use for I<sup>2</sup>C communication?

### Questions from LAB 5 documentation
1. What is the difference between a parallel and serial communication?
2. What is the difference between synchronous and asynchronous communication?
3. Explain endianness
4. Which instruction within the Serial Library waits for the serial transmission to complete?
5. What is the first message always in the I<sup>2</sup>C communication?
</details>

<details>
<summary>Lab 6 - click to expand / close</summary>

## Lab 6

### Questions from LAB 7 (Analog Signals Proc.) documentation

1. What is the difference between analog and digital signals?
2. What formula would you use to calculate the digital value provided by an ADC? (V<sub>ref</sub>, ADC_reading, Voltage_measured)
3. What function would you use to read a value from an ADC?
4. What should you do when switching between readings from several inputs so that the next input wouldn't be noisy?
5. What do you need to make sure of when configuring the pins so that the ADC reading would work properly?
5. What method (not function) is used for sampling?
</details>