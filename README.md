# ShoeManagmentSystem
The Shoes Management System is an assembly language program designed to manage shoe inventory and sales. It tracks stock, calculates total sales, and displays statistics for different shoe categories. This project demonstrates the use of assembly language for inventory management and sales tracking.

# Features
Inventory Management: Tracks the stock of shoes in different categories.
Sales Calculation: Calculates total sales based on user purchases.
Statistics Display: Provides detailed statistics for shoe categories and sales.
# Inputs and Outputs
Input: User's selection of shoe categories and quantities.
Output: Updated inventory, total sales, and category statistics.
# Where to Run
# emu8086
This program was tested on the x86 emulator emu8086. You can use emu8086 to run and debug the code.

# Visual Studio Code
You can also run this assembly program in Visual Studio Code. Follow the steps below to set up and run assembly code in VS Code:

Install Visual Studio Code: Download and install Visual Studio Code from here.

Install MASM or TASM: Ensure you have MASM or TASM installed on your system to assemble and link the code.

Install the Code Runner Extension:

Open Visual Studio Code.
Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window.
Search for "Code Runner" and install it.
Set Up Your Workspace:

Create a folder for your assembly project.
Place your .asm files in the folder.
Configure Tasks:

Create a tasks.json file in the .vscode folder inside your project directory.
Add the following configuration to assemble and run your assembly code:
```json
{
  "version": "2.0.0",
  "tasks": [
    {
      "label": "Build Assembly",
      "type": "shell",
      "command": "ml",
      "args": ["/c", "/coff", "${file}"],
      "group": {
        "kind": "build",
        "isDefault": true
      }
    },
    {
      "label": "Run Assembly",
      "type": "shell",
      "command": "link",
      "args": ["/subsystem:console", "${fileBasenameNoExtension}.obj"],
      "group": {
        "kind": "build",
        "isDefault": true
      }
    }
  ]
}
```
Run Your Code:

Open your .asm file in Visual Studio Code.
Press Ctrl+Shift+B to build the assembly code.
Run the executable file generated in the terminal.
Remarks
Ensure the code is thoroughly tested before running.
This project is a practical example of using assembly language for inventory and sales management.
# Contributor
# Abdul Wasay Tabba 
