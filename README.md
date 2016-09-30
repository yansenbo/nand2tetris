# nand2tetris

![nand2tetris](http://nand2tetris.org/banner.png)  

Introduction
------------

This project will build a Modern Computer from First Principles Using HDL(Hardware Description Language), refer from http://nand2tetris.org/

Table of Contents
---

- [Project 1: Elementary Logic Gates](#project1)
    - [Resources](#resources)

## Project1
The interface of `Nand` is:
```
Nand(a= ,
     b= ,
     out= );
```
<u>We can build:</u>

-  **Not(a) = Nand(a,a)** 
-  **And(a,b) = Not(Nand(a,b))** 
-  **Or(a,b) = Not(And(Not(a), Not(b)))** 

building elementary logic gates listed below based on `Nand`

|Index|Chip(HDL)|Description|Test Script|Compare FIile|
|---|---|---|---|---|
|0.|Nand|Nand gate(primitive)|
|1.|Not|Not gate|Not.tst|Not.cmp|
|2.|And| And gate|    And.tst| And.cmp|
|3.|Or|  Or gate| Or.tst|  Or.cmp|
|4.|Xor| Xor gate|    Xor.tst| Xor.cmp|
|5.|Mux| Mux gate|    Mux.tst| Mux.cmp|
|6.|DMux|    DMux gate|   DMux.tst|    DMux.cmp|
|7.|Not16|   16-bit Not|  Not16.tst|   Not16.cmp|
|8.|And16|   16-bit And|  And16.tst|   And16.cmp|
|9.|Or16|    16-bit Or|   Or16.tst|    Or16.cmp|
|10.|Mux16|   16-bit multiplexor|  Mux16.tst|   Mux16.cmp|
|11.|Or8Way|  Or(in0,in1,...,in7)| Or8Way.tst|  Or8Way.cmp|
|12.|Mux4Way16|   16-bit/4-way mux|    Mux4Way16.tst|   Mux4Way16.cmp|
|13.|Mux8Way16|   16-bit/8-way mux|    Mux8Way16.tst|   Mux8Way16.cmp|
|14.|DMux4Way|    4-way demultiplexor| DMux4Way.tst|    DMux4Way.cmp|
|15.|DMux8Way|    8-way demultiplexor| DMux8Way.tst|    DMux8Way.cmp|

### Resources
- [Chapter 1](http://www.nand2tetris.org/chapters/chapter%2001.pdf) of *The Elements of Computing Systems*.
- [Appendix A: Hardware Description Language (HDL)](http://www.nand2tetris.org/chapters/appendix%20A.pdf) of *The Elements of Computing Systems* (use as technical reference, when needed)
- [HDL Survival Guide](http://www.nand2tetris.org/software/HDL%20Survival%20Guide.html), written by Mark Armbrust (use as technical reference, when needed)
- [FAQ](https://www.coursera.org/learn/build-a-computer/supplement/Dkosx/faq)