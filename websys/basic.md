# This document handles the basic 
> 2026.09.01

## computer components
### Hardware

**CPU** 
- Arithmetic Logic Unit  
> performs arithmetic and logical operations
- Control Unit
> decodes instruction
> set up ALU with data from memory (ROM/ RAM)
- Registers
> small, fast memory in cpu  
> temporarily holds data & instruction  
> Accesiblle data access by ALU

. . .

**RAM/ROM**
- RAM (Random Access Memory)
> volatility   
> accessed by cpu  
> holds the current program and data  
> free read and write  
- ROM (Read Only Memory)
> parmanet  
> only reading  
> Stores firmware( start computer with default setting  

### Software

**OS | Operating System**  
The programs that control, supervise, and support a computer system's hardware and application software  
~~without OS, computer can not work at all~~

**Types of OS**
- Application SW  
> users perform various task  

- System SW  
> The program allows users to manage hard ware  
> execute application sw, manage files and data  
> e.g OS, langyage compiler  

**Main function of OS**
- manage hardware to achieve the best use and performance by the application SW
 > scheduling of resources
 > excute application SW on HW device
- provide user-friendly interfaces
- provides valuable services for the users
 > sharing program data
 > recovering error

**OS components**  
- processor manager  
> control operation of CPU  
> Includes Scheduler that arranges the execution of program  
- memory manager  
> control data storage in main memory (RAM)  
- file manager  
> Manages the files system on secondary storage - directories and files  
- device manager  
> coordinate peripheral device  

**Interface**
- GUI | Graphic user interface
> Based on WIMPS (windos, Icons, Menus and pointer)
- CLI | command-line interface
> 
## ASCII
**American Standard Code of Information Interchange**  

## Number System
- Decimal
> 0 to 9, base 10
- Binary
> 0,1 | base 2
- hexadecimal
> 0to9,A,B,C,D,E,F | base 16
- Octal
> 0to7 | base 8


## Data organisation
A binary digit 0 or 1 -> called bit  
String of 8bit = 1byte

**Data hierachy**
- data filed
> the most smallest amount of meaningful data showing attribute (column | name, or an address)
- data record
> A collection of related data fileds, describe single entitiy or item (row)

<img width="707" height="308" alt="image" src="https://github.com/user-attachments/assets/ae1146e4-c557-4ffc-b66b-c7a3d9909c8c" />  

*reference: [Computer Science IGCSE - Chapter 13 Databases](https://computerscienceigsce.wordpress.com/chapter-13/)*

- data table/file
> A gouping of related data records
- database
> A system where all related data files are grouped together for organized storage and access

**Data Measurement**
- kilobyte (KB, 1024 byte)
- Megabyte (MB, 1024 KB)
- Gigabyte (GB, 1024 MB)
- Terabyte (TB, 1024 GB)
- Petabyte (PB, 1024 TB)

**Exact vs approximate**

| Unit | Exact value (binary) | Approximately (decimal) | Difference |
|------|---------------------|-------------------------|------------|
| KB   | 2^10 = 1,024 bytes | 10^3 = 1,000 bytes | 2.4% |
| MB   | 2^20 = 1,048,576 bytes | 10^6 bytes | 4.9% |
| GB   | 2^30 = 1,073,741,824 bytes | 10^9 bytes | 7.4% |
| TB   | 2^40 bytes | 10^12 bytes | 10.0% |
| PB   | 2^50 bytes | 10^15 bytes | 12.6% |

"Approximately" applies only to the decimal column.
The binary value is exact by definition; the decimal one is rounded for convenience.


**KB < MB < GB < TB < PB (KMGTP)**

> why 1024?
> Computer is based on binary → memory size can only be 2ⁿ
> Among these, 2¹⁰ = 1024 is the closest to 1000 (kilo)
> Error: KB 2.4% → GB 7.4% → PB 12.6% -> reason why it

## Boolean algebra
> not A -> $\bar{A}$ $A'$

> boolean table  
> <img width="1417" height="918" alt="image" src="https://github.com/user-attachments/assets/b6d8b1ea-4d6a-472f-91c7-afc7d56891a4" />  
> src : (https://youtu.be/lKqTSBKmWA4)  
> . . .  
> https://youtu.be/lKqTSBKmWA4?si=MD-5EwQ6dUQOaVaP  
> https://youtu.be/5NGKbiA04Cw?si=KgWuq0X7NKLcneHX

