# cmos-nand-gate-on-magic-VLSI  
## Introduction to Magic VLSI:
Magic is a Very-large-scale integration (VLSI) layout tool originally written by John Ousterhout and his graduate students at UC Berkeley.
 Magic VLSI is a open source software for physical chip layout.Magic currently runs under **Linux**, although versions exist for DOS, OS/2, and other operating systems.  
 Magic is frequently used in conjunction with **IRSIM** and other simulation programs.  
 I would recommend to get Magic VLSI from the latest sources:https://github.com/libresilicon/magic-8.2   
 and also check these websites for further details:  
  http://opencircuitdesign.com/magic/  
  http://vlsi.csl.cornell.edu/magic/  
  http://www.research.digital.com/wrl/magic/magic.html  
 In order to open the layout of a cell, do the following:  
 1. **For starting up magic:** Magic uses its own internal ASCII format for storing cells in disk files. Each cell name is stored in its own file, named **name.mag**.    
* The first line in a **.mag** file is the string to identify this as a Magic file.  
**magic**  
* The next line is optional and is used to identify the technology in which a cell was designed. If present, it should be of the form  
**tech** techname (the technology we used is ***scmos** and **sample6m**)  
*  If absent, the technology defaults to a system-wide standard, currently **nmos**.  
2. **For selecting a file:** In the top menu-bar select File > Open and navigate to one of the *.mag files from the examples, e.g. nandgate.mag  
3. Select a *.mag file and click Open. The layout of the selected cell will be show in the main window called **top level**  
4. **For editing the layout:** you can edit the layout by entering commands in the command window called **tkcon 2.3 main**  
5. Further tutorials for Magic can be found here http://opencircuitdesign.com/magic/tutorials/tut1.html.  
## CMOS NAND GATE:  
The below figure shows a 2-input Complementary MOS NAND gate. It consists of two series NMOS transistors between Y and Ground and two parallel PMOS transistors between Y and VDD.  
If either input A or B is logic 0, at least one of the NMOS transistors will be OFF, breaking the path from Y to Ground. But at least one of the pMOS transistors will be ON, creating a path from Y to VDD.  
 Hence, the output Y will be high. If both inputs are high, both of the nMOS transistors will be ON and both of the pMOS transistors will be OFF. Hence, the output will be logic low.  
 # Designing a CMOS NAND GATE on magic VLSI layout tool:  
 Below is the picture of the nandgate I designed:  
 ![alt text](https://github.com/qurratulainalam/cmos-nand-gate-on-magic-VLSI/blob/master/nand%20gate%20picture.png)  
 
