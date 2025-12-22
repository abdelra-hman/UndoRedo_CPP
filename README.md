# Undo/Redo Implementation using Stack in C++



## Overview
This project demonstrates a simple **Undo/Redo system** in C++ using the standard library stack (`std::stack`).  
The class `clsMyString` stores a string value and allows undoing or redoing changes.

### Core Features
- `Value` – Property to get/set string value  
- `Undo()` – Revert to the previous value  
- `Redo()` – Reapply the last undone value  

### How It Works
1. Setting a new value pushes the old value onto the **Undo stack**.
2. Calling `Undo()` pops from the Undo stack to revert the value and pushes the current value to **Redo stack**.
3. Calling `Redo()` pops from the Redo stack to restore a value and pushes the current value to Undo stack.

---

## Files in the Repository
