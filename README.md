# # 16-Bit CPU
This is a Logisim-based 16-bit CPU that supports a set of instructions for performing arithmetic and logical operations, data memory access, and control flow. The CPU architecture includes 8 general-purpose registers, two separated memory spaces for data and instructions, and a set of control signals that enable the execution of the supported instructions.

### Supported instructions
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Format</th>
      <th>Functionality</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>li</td>
      <td>li $r1, x</td>
      <td>load immediate number to one register ($r1)</td>
    </tr>
    <tr>
      <td>add</td>
      <td>add $r1, $r2, $r3</td>
      <td>add two register numbers ($r2 and $r3) and store the result in one register ($r1)</td>
    </tr>
    <tr>
      <td>and</td>
      <td>and $r1, $r2, $r3</td>
      <td>bit-wise logical AND of two register numbers ($r2 and $r3), and store the result in a register ($r1)</td>
    </tr>
    <tr>
      <td>or</td>
      <td>or $r1, $r2, $r3</td>
      <td>bit-wise logical OR of two register numbers ($r2 and $r3), and store the result in a register ($r1)</td>
    </tr>
    <tr>
      <td>load</td>
      <td>ld $r1, $r2</td>
      <td>load a 16-bit number from data memory to a register ($r1). The data memory address is the value in a register ($r2)</td>
    </tr>
    <tr>
      <td>store</td>
      <td>st $r1, $r2</td>
      <td>load a 16-bit number from a register ($r1) to data memory. The data memory address is the value in a register ($r2)</td>
    </tr>
    <tr>
      <td>move</td>
      <td>move $r1, $r2</td>
      <td>copy the value of one register ($r2) to another register ($r1)</td>
    </tr>
    <tr>
      <td>addi</td>
      <td>addi $r1, $r2, x</td>
      <td>add a register number ($r2) and an immediate number (x), and store the result in one register ($r1)</td>
    </tr>
  </tbody>
</table>

### Usage
<img src="https://ibb.co/rxRkkJ2" alt="cpu_image">

<table> <tbody> <tr> <td>Open Logisim.</td> </tr> <tr> <td>Open the CPU.circ file in Logisim.</td> </tr> <tr> <td>To load a program, use 'Ctrl+O' shortcut and select the .circ file</td> </tr> <tr> <td>To run the program, go to "Simulate" &gt; "Ticks Enabled".</td> </tr> <tr> <td>To reset the CPU, go to "Simulate" &gt; "Reset Simulation".</td> </tr> </tbody> </table>


