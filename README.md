# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**

module upcounter(clk,rst,count); input clk,rst; output reg[3:0]count; always@(posedge clk or negedge rst) begin if(!rst) count <= 4'b0000; else count <= count+1; end endmodule

 Developed by:SHALINI .I RegisterNumber:25015951
**RTL LOGIC FOR 4 Bit Ripple Counter**
![Image 2025-12-18 at 8 47 52 PM](https://github.com/user-attachments/assets/b3619504-aa95-4a25-91b6-83519bce49b3)

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
![Image 2025-12-18 at 8 48 31 PM](https://github.com/user-attachments/assets/d90fb39d-7578-4aa0-81b3-5f817958fcf7)

**RESULTS**
Thus 4-BIT-RIPPLE-COUNTER is verified successfully.
