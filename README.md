NAME:GAYATHRI M

REG NO:212224050007
# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
~~~
module experiment2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~a)&(~b)&(~c)&(~d))|(a&(~c)&(~d))|(~b)&c&(~d)|((~a)&b&c&d)|(b&(~c)&d);
assign f2=(x&(~y)&z)|((~x)&(~y)&z)|((~w)&x&y)|(w&x&(~y))|(w&x&y);
endmodule
~~~

**Logic symbol & truth table:**

![Screenshot 2025-03-21 223919](https://github.com/user-attachments/assets/15023dd3-896e-4b18-b10f-102abbcd010e)

![Screenshot 2025-03-21 223939](https://github.com/user-attachments/assets/e89d91f5-37f3-474d-898d-80c4a3710e46)

**RTL Realisation:**

![Screenshot 2025-03-19 131726](https://github.com/user-attachments/assets/a6b5e720-cf7a-40d4-a9a7-a3cb38afc4e0)

**RTL Waveform:**

![Screenshot 2025-03-19 132449](https://github.com/user-attachments/assets/3e6fbaf7-dec4-4f5e-9e59-6fd98522f4e9)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

