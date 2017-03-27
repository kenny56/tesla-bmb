# tesla-bmb
disassembly of the SiLabs 8051F530A code
i have organized this code as 133 separate functions or subroutine elements.
i have identified the function or purpose for 125 of these elements, leaving about 8 more to do.
See the flow_outline .pdf file for top-level subroutine list.

There are generic compiler-generated routines, sometimes duplicates.  i will try to identify and
mark those over time.  Likely a keil C compiler was used.

01B1;
025C;
02F3;
0B52;
0ED7;
1230;

Interesting Finds:

the CRC-8 is done using a look-up table at 0C15;  
the data bytes at 0B74 are the bq76 Register 00 status words;  
sending x79 out the UART is a request to the BMS to reset the bq76;  
Flash Lock and Key routine at 084D;  
