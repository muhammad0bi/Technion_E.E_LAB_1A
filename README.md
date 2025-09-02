Space Invaders Game

This project is a hardware implementation of the classic Space Invaders game using SystemVerilog and the Quartus development environment.
The game runs on an FPGA, with user inputs provided through physical buttons or switches connected to the FPGA.

Tools and Technologies Used
  -Quartus for FPGA development.
  -SystemVerilog for hardware design.
  -TCL scripts for pin assignment and integration.
  -Bitmap graphics for visual display.
  -FPGA board for deployment and testing.

Project Description
  -We used TCL scripts to map the FPGA’s physical inputs and KBD inputs to logical inputs in our Quartus project. These inputs are used to control the
   game (e.g., movement and shooting).
  -The game logic, including player and monester behavior, was written in SystemVerilog and deployed onto the FPGA.
  -Bitmaps were used to visually render game objects like the player, monster, missiles, and shields.

Game Features
  -The player can move left and right and launch missiles.
  -Missiles increase in speed as the game progresses.
  -The goal is to destroy all monster particles by hitting them with missiles.

Monster
  -Move left and right and gradually progress toward the player.
  -Their movement speed increases as the game progresses.
  -Can shoot missiles at the player.
  -The player loses the game after being hit three times.
  -Monster change color when injured (blue → yellow → red) and eventually get destroyed.
  -Occasionally, a random healing rescue pill appears, If an injured monster particle collects the pill in time, it can recover.
   If not, the monster particle continues to take damage or is eventually destroyed after a specific time.
  -Shields are placed in front of the player, which can absorb monster missiles but get damaged after many hits and eventually destroyed.

Sound effects are triggered when missiles are launched or hit targets.

A score counter and life bar are included in the game.
