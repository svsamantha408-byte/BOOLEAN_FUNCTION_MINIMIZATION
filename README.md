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
module ex2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module f2_logic(w, x, y, z, f2_out);
    input w, x, y, z;
    output f2_out;
    wire w1, w2, w3;
not(yn, y);

    and(w1, yn, z); // y'z
    and(w2, y, x);  // yx
    and(w3, y, w);  // yw

    or(f2_out, w1, w2, w3);
    endmodule


Developed by:Samantha Shree SV
RegisterNumber: 25017585*/


**RTL realization**
<img width="1920" height="1080" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/cdb9ea0c-9eec-4765-8f40-9dbaec3887cf" />

<img width="1920" height="1080" alt="Screenshot (95)" src="https://github.com/user-attachments/assets/c76119f7-cd26-43c4-b9a4-89facd5b9757" />

**Output:**
<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/cac62679-5f93-4ec6-9be8-e48d0727cd78" />

<img width="1920" height="1080" alt="Screenshot (96)" src="https://github.com/user-attachments/assets/ea21332a-d0e3-441c-bf15-0fffa31dcdd7" />


**RTL**


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

