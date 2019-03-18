# electrostatic-adhesion-plate

#### Motivation

The motivation behind this project is that I wanted to test how strong [electro-adhesion](https://en.wikipedia.org/wiki/Electroadhesion) really is and what clamping force I can get myself with it. Since PCBs are very inexpensive nowadays, the choice fell on electrodes directly on a circuit board. In the first version (100x100mm) the electrode gap is not yet optimal and there are points where corona discharges are likely, this is fixed in the second version (DinA5). 

A batch (50pcs) of the seccond version is about to be ordered by me.

#### Design

![Design](/Images/b69c3fc8-82f3-4f2c-8ecb-c5ef68ff4d3b.jpeg)

The boards were designed so that they can be connected to larger printed circuit boards (electrically) using solder connections. This makes it possible to build relatively large electroadhesive surfaces with relatively inexpensive printed circuit boards.

![Solderpoints](/Images/f03ba77f-4d8d-44b8-966d-36029fc7bf42.jpeg)

The surface of each PCB or the whole panel should be coated with a high voltage isolator, as the soldermask does not withstand high voltage very well. Kapton is a suitable material as its dielectric strength is about 7.6kV/25µm, unfortunately it is difficult to apply. 
Another solution which is being tested is PlastiDip. PlastiDip has a much lower dielectric strength 1.6kV/25µm, so it has to be applied thicker. The advantage here is the rubber-like surface which generates a higher shear force due to its friction.

[Demo of Kapton and PlastiDip (twitter link)](https://twitter.com/JanHenrikH/status/1094664006059593729)

The electrode voltage should be between 500V and 5kV DC (depending on the design), whereby a higher voltage means a higher holding force. This voltage can be obtained from any cheap DC high voltage source (e.g. a bug zapper) or from a low AC voltage source (Please do not use direct mains voltage). The AC voltage can be multiplied and rectified by the Cockcroft Walton voltage multiplier on the back of the PCB.

![Solderpoints](/Images/b7234b52-5d54-4049-b951-56b2e7e6c978.jpeg)

___

## [100mm * 100mm](100100mm/)

| Parameter         | Value         | 
| -------------     |:-------------:|
| Electrode Voltage | 500V-2000V    |
| Electrode Voltage*| 500V-3000V    |
| without extra coating (silkscreen)|
| shearing force    | 9N @1.4kV     |
| shearing force cm²| 90mN/cm² @1.2kV|
| adhesive force    | **            |
| PlastiDip Coating                 |
| shearing force    | 4N @1.4kV     |
| shearing force cm²| 40mN/cm² @1.2kV|
| adhesive force    | **            |
| Kapton Coating                 |
| shearing force    | 2.5N @1.4kV     |
| shearing force cm²| 25mN/cm² @1.2kV|
| adhesive force    | **            |

\* With Insulation

\** TBD

#### [Demo Video](https://twitter.com/JanHenrikH/status/1094664006059593729)

![Frontview](/100100mm/Front.png)

___

## [DIN A5](DINA5)

| Parameter         | Value         | 
| -------------     |:-------------:|
| Electrode Voltage | 500V-2000V    |
| Electrode Voltage*| 500V-5000V    |
| shearing force    | **            |
| adhesive force    | **            |

\* With Insulation

\** TBD

#### Changes to V1 (100100mm)

 * Size is now 148*210mm (DinA5)
 * Electrode width and distance are optimized
 * M3 threads where added
 * Sharp edges where removed

![Frontview](/DINA5/Front.png)

### [5050mm](DINA5)

| Parameter         | Value         | 
| -------------     |:-------------:|
| Electrode Voltage | 500V-2000V    |
| Electrode Voltage*| 500V-5000V    |
| shearing force    | 600mN         |
| shearing force cm²| 6mN/cm² @1.2kV|
| adhesive force    | **            |

\* With Insulation

\** TBD

![Frontview](/5050mm/Front.png)

