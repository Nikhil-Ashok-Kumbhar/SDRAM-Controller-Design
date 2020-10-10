# SDRAM-Controller-Design

Overview:
The goal of this project is to design an SDRAM controller that allows SDRAM memory to be interfaced
with a microprocessor having only asynchronous memory support. There is no requirement to build
the hardware, but a complete written report containing schematics and theory of operation is
required.


➢ Detailed Requirements:
The SDRAM controller should be designed to interface with one or more SDRAM memory devices. The
minimum requirement is that support for a single MT48LC4M16A2 be provided. It is strongly
suggested that you attempt to provide interfacing with the 80386DX processor, but you may interface
with another 32-bit data bus processor provided SDRAM memory support is not already provided for
that processor.
• The detailed requirements follow:
1. Support the MT48LC4M16A2 memory device is required.
2. Support for an 80386DX or similar processor with 32-bit data bus not having SDRAM support is
required.
3. The use of “northbridge/MCH/IMCH” chipsets, SDRAM controllers (including reference design or
commercial FPGA/CPLD/ASIC/hard copy solutions are not allowed).
4. A complete controller solution including state machine, row, column, and bank signal generation,
data masking, data flow, ready logic, and refresh support must be provided.
5. Interfacing with ~ADS, W/~R, and M/~IO control signals (or equivalent) will be required.
6. Support the sending of AUTO REFRESH commands at a rate sufficient to ensure memory integrity.
Steps to minimize microprocessor waiting due to refresh will be worth more credit.
7. Support the READY logic of the selected microprocessor system, especially when refresh is
occurring, unless a bus locking protocol is used.
8. Support is only required for burst length 2 transfers, although you may add higher burst length
support for DMA operations if you wish for extra credit or support lower bit-width memories with
higher burst lengths as an option.
9. Extra credit steps:
a. Adding hardware external I/O control pins to support variable timing, with changes in both the
FSM timing and the LMR values being loaded.
b. Adding hardware external I/O to support 4- and 8-bit wide memories with burst lengths of 8
and 4 appropriately with all changes needed to the FSM and SDRAM interface
