# Open2DJ

A modernization of project for the memories of childhood

## Old Machine Specification

This specification is from the machine that I currently own. It depends on EZ2** version to be run, however, I focus on the 1st ~ BErA in this repository. I tested AEIC and EC on this machine, they also worked fine.

### PC Specification

See [PC Specification](docs/PC_SPECS.md)

### Control Card

See [Control Card](docs/CONTROL_CARD.md)

### IO Board

See [IO Board](docs/IO_BOARD.md)

## Plan

Hardwares are no longer manufactured, or supported for any interruptions due to original manufacturer closed their business or discontinued their products. To keep the game running in future, several hardware components (Control Card, IO Board, Hardlock, ...) should be modified or transformed into softwares to maximize compatiability for modern hardware and operating systems. (especially Hard drive; PATA -> SATA can be a good transition)

* Control Card : USB-based controller will be appropriate for this project, however, there are input timing issues.
* IO Board : This should be integrated with Control Card. Some of ports should be changed or removed to make suitable for home arcade environment, customized controllers.
* Hardlock : This is the most sensitive issue in this project; I do not release any contents or dumps of existing hardlocks. I will work on extracting and emulating hardlocks to run the games without them, to keep physical hardlock device to store somewhere else. This is not for pirates, but for collectors who want to preserve precious heritages.

Operating system should be at least Windows 2000, or Windows XP. I already checked the games run in such systems. 

### Procedures

* Reversing and Rewriting Requirements
* Build testing applications and utilities in old environment (Windows 9x)
* Build instrumentalized toolset in old environment
* Migrate into modern environment (Windows NT 5.x ~)

### Expected Products

* License Dumping Application for HASP E-Y-E
* A 9x/NT Kernel Driver and Utilities for Hardlock Emulation
* A 9x/NT Device Driver and Utilities for Control/IO Connectivity
