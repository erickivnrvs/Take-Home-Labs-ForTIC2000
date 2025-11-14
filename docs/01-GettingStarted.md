# 01 - Getting started with the C2000 Delfino F28379D Launchpad Development Kit

## About the board
"LaunchPad" is the physical development board. We can think of it as a whole system that supports and allows us to interact with the microcontroller on board.
## Characteristics
* Low cost: Low cost board for the Delfino F2837xD microcontrollers. Includes the required hardware and software to begin developing applications.

* Integrated depuration: On board JTAG depurator (XDS100v2). This allows the board to be interfaced directly to a computer for programming and data I/O under a single USB connection.

* Easy communication: Besides JTAG, the USB connection allows to communicate with the board under a serial protocol(UART).


## About the Microcontroller: TMS320F28379D


* Proccesing architecture: Dual Core Architecture. Integrates two C28x CPU of 32 bits, each one runnning at 200MHz. This allows the board to split tasks between cores.

* Co-Processing Accelerators(CLA): Besides the main Dual Core Processors, the microcontroller incorporates two programable Law Control Accelerators(CLA). These 32 bits independent processors, also running at 200MHz with floating point and running parallel to the main CPUs are suitable for high frequency and intensive use of mathematic functions, allowing the CPUs to focus on other tasks.

* Powerful Mathematics Unit(Key for Matlab/Simulink implementations): Each C28x main CPU includes a Floating Point Unit(FPU) of simple precision, and a Trigonoetric Mathematics Unit (TMU). The generated code by Simulink to perform floating point or trigonometrics operations is executed on real time, rather than being emulated by software. 

* Analog Inputs (Sensing): Incorporates up to 4 independent Analog to Digital Converters(ADCs) which can operate either at 16 bits mode or 12 bits high speed mode.

* Analog Outputs: Integrated with 24 standard PWM channels, with 16 of them as High Resolution PWM.

* Digital to Analog Converters: Includes three DAC outputs to generate analog signals.

* Communicaction: Includes standard protocols for communication and interaction with external devices

    USB 2.0 

    CAN

    SPI

    I2C

    SCI (UART)
