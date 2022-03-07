# 6T SRAM Cell

## Abstract
Since there is an ever increasing demand on battery operated portable devices, the rate of power consumption has become a major issue. To maintain a long battery life, the power consumption has to be managed in an appropriate way. One such aspect is of the SRAM cell, the basic unit of memory in cache. The conventional design of an SRAM cell is not good enough since it consumes a lot of power. That is where low power VLSI techniques come into picture. The MTCMOS technique has been applied on a 6T SRAM cell to evaluate the performance and the power consumption. MTCMOS uses two sleep transistors which have a higher threshold voltage to cut off the power supply to th SRAM cell when it is not being used.

## Reference Circuit Details
The MTCMOS SRAM circuit consists of a conventional 6T SRAM cell along with two sleep transistors which have a higher threshold voltage. These sleep transistors are controlled by two signals, CLK, and nCLK, which is the complement of CLK. A subcircuit for CMOS inverter is constructed using a PMOS and an NMOS. This subcircuit is used to invert the CLK signal to form nCLK. When CLK is high, the transistors are on, connecting the virtual power rails to the physical power rails. In this mode, any read or write operation can be done. But when CLK is low, the sleep transistors are turned off. Now the virtual rails are powered by the data present in the SRAM cell through the pass transistors of the corresponding inverters. In this mode no operation can be performed to the SRAM cell, and it only retains the data. For read and write operations the signals, word line WL, bit line BL, and the complement of bit line nBL are used. When CLK and WL are high the read and write operations can be performed. To prevent loss of data, it has been made sure that WL is never high when CLK is low. In the sleep state, the charge in the SRAM cell can leak out slowly since it is not connected to the power supply. So the sleep transistors have to be turned back on before the charge can leak and change the state of the SRAM. Hence the frequency of CLK has been chosen accordingly. The sleep transistors are given a higher threshold voltage so that the leakage would be less and more power would be con served. The threshold voltage is increased by applying a substrate bias voltage to the sleep transistors.

## Implemented Circuit Diagram

## Implemented Circuit Waveforms
