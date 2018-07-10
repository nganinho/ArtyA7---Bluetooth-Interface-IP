# bluetooth-interface-ip
Reference Documents:
https://reference.digilentinc.com/_media/pmod:pmod:pmodBT2_rm.pdf 
https://reference.digilentinc.com/reference/pmod/pmodbt2/reference-manual


IP Specification and Status of implementation
Build the bluetooth control IP ( non-processor version )
1. RX mode (Slave mode)
 - Receive the package which is transfered by HC05 from smartphone
 - Decode the control of data and perform specific actions
 - HC05 automatically paired with smartphone after click connecting via smartphone application
 - UART mode: 9600bps, 1 Start, 1 Stop, No Parity

2. TX mode (Not yet)
 - Transfer data to HC05 as feedback or control data
 - Configure the HC05
 
3. IP control and interface (Not yet)
 - AXI interface with processor
 - Internal register to define operation options
 - Internal FIFO to store TX/RX data. Block size can be 128 or 64 bytes.

4. Bluetooth configuration (Not yet)
 - Configure HC05 module via AT commands
 - Change the baudrate (default: 9600)
 - Change the password (default: 1234)

5. Applications (Not yet)
 - Robot control
 - IO control (LED, Lamp, another purpose)
 - MP3 player (with additional hardware needed)
