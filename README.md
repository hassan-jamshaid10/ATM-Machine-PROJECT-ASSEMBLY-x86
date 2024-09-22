# ATM Machine Project

## Overview
This project is an implementation of an **ATM machine** in **Assembly x86**, utilizing interrupts for system operations. The ATM machine simulates real-world ATM functionality, such as checking balance, withdrawing money, depositing money, and changing the PIN.

## Features
- **Check Balance**: View the current balance of the account.
- **Withdraw Funds**: Withdraw a specified amount from the account (with error handling for insufficient funds).
- **Deposit Funds**: Deposit a specified amount into the account.
- **Change PIN**: Securely change the PIN of the account.
- **Exit**: Safely exit the ATM system.

## Technical Details
- Written in **Assembly x86** using interrupts (`INT`).
- The project uses low-level programming and direct interaction with the system hardware to handle user input, screen display, and data storage.
- Includes a simple text-based interface for ease of interaction.

## How to Run

### Prerequisites
1. **Assembler**: You need an x86 assembler such as **NASM** (Netwide Assembler) or **MASM** (Microsoft Macro Assembler).
2. **x86 Emulator or Real Machine**: You can use an emulator like **DOSBox**, **QEMU**, or run directly on an x86-compatible machine.

### Steps to Run:
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/atm-machine-assembly-x86.git
    cd atm-machine-assembly-x86
    ```
2. Assemble the code using NASM or MASM:
    ```bash
    nasm -f bin atm.asm -o atm.com
    ```
3. Run the executable using an emulator or real hardware:
    - **In DOSBox**:
      ```bash
      dosbox atm.com
      ```
    - **On real hardware**: Copy the executable to a bootable drive and run it.

## Usage
- When you start the ATM machine, you will be prompted to enter your PIN.
- Navigate through the options to:
  - Check your account balance.
  - Withdraw or deposit money.
  - Change your PIN for security.
- All inputs are handled via the keyboard, and the outputs are displayed in a simple text format.

## Screenshots
_Add screenshots or ASCII representations of the interface._

## Interrupts Used
The project makes extensive use of **software interrupts** for handling system calls, such as:
- **INT 21h**: For handling I/O operations, like reading user input and printing to the screen.
- **INT 10h**: For screen control.
- **INT 16h**: For keyboard input.

## Future Enhancements
- Implementing support for multiple accounts.
- Adding error handling for invalid inputs or PIN attempts.
- Implementing transaction logs and history tracking.

## Contributing
Feel free to fork the repository, submit pull requests, or report issues.

## Contact
For any inquiries or issues, please contact hjamshaid81@gmail.com
