Sudoku Solver
An automated Sudoku solving application built in C++ using backtracking algorithm with input validation and performance metrics.
🎯 Features
Multiple Input Modes:
Hardcoded default puzzle
File-based input (input1.txt)
Manual console input
Input Validation: Ensures puzzle correctness and detects conflicts before solving
Solution Analysis:
Determines if puzzle has unique solution
Detects multiple solutions
Identifies unsolvable puzzles
Backtracking Algorithm: Efficient recursive solver using constraint satisfaction
Formatted Output:
Structured console display
Text file export (output.txt)
Styled HTML export (output.html)
Performance Metrics: Measures and displays execution time using <chrono> library
🛠️ Technologies Used
Language: C++
Compiler: g++ / Visual Studio
Libraries:
<iostream> - Console I/O
<fstream> - File handling
<sstream> - String manipulation
<chrono> - Execution time measurement
📋 How to Run
Prerequisites
C++ compiler (g++, GCC, or Visual Studio)
Compilation
Linux/Mac:
g++ sudoku_solver.cpp -o sudoku_solver
./sudoku_solver
Windows (Command Prompt):
g++ sudoku_solver.cpp -o sudoku_solver.exe
sudoku_solver.exe
Windows (Visual Studio):
Open Visual Studio
Create new C++ project
Add sudoku_solver.cpp to project
Build and run (F5)
Input Options
When you run the program, you'll see:
========== SUDOKU SOLVER ==========

Select Input Method:
1. Hardcoded Default Puzzle
2. Load from File (input1.txt)
3. Manual Input

Enter your choice (1-3):
📊 Sample Input Format
For File Input (input1.txt):
5 3 0 0 7 0 0 0 0
6 0 0 1 9 5 0 0 0
0 9 8 0 0 0 0 6 0
8 0 0 0 6 0 0 0 3
4 0 0 8 0 3 0 0 1
7 0 0 0 2 0 0 0 6
0 6 0 0 0 0 2 8 0
0 0 0 4 1 9 0 0 5
0 0 0 0 8 0 0 7 9
Note: Use 0 for empty cells
📤 Output Files
The program generates two output files:
output.txt - Plain text format with solved puzzle
output.html - Styled HTML page for viewing in browser
🧪 Example Output
========== SUDOKU SOLVER ==========

Original Puzzle:

+-------+-------+-------+
| 5 3 . | . 7 . | . . . |
| 6 . . | 1 9 5 | . . . |
| . 9 8 | . . . | . 6 . |
+-------+-------+-------+
| 8 . . | . 6 . | . . 3 |
| 4 . . | 8 . 3 | . . 1 |
| 7 . . | . 2 . | . . 6 |
+-------+-------+-------+
| . 6 . | . . . | 2 8 . |
| . . . | 4 1 9 | . . 5 |
| . . . | . 8 . | . 7 9 |
+-------+-------+-------+

Validation: PASSED ✓
Solution Analysis: Unique solution ✓

Solving...

✓ PUZZLE SOLVED SUCCESSFULLY!

Solved Puzzle:

+-------+-------+-------+
| 5 3 4 | 6 7 8 | 9 1 2 |
| 6 7 2 | 1 9 5 | 3 4 8 |
| 1 9 8 | 3 4 2 | 5 6 7 |
+-------+-------+-------+
| 8 5 9 | 7 6 1 | 4 2 3 |
| 4 2 6 | 8 5 3 | 7 9 1 |
| 7 1 3 | 9 2 4 | 8 5 6 |
+-------+-------+-------+
| 9 6 1 | 5 3 7 | 2 8 4 |
| 2 8 7 | 4 1 9 | 6 3 5 |
| 3 4 5 | 2 8 6 | 1 7 9 |
+-------+-------+-------+

Execution Time: 2.45 ms

Results saved to output.txt
HTML results saved to output.html
🧠 Algorithm Overview
The solver uses Backtracking - a recursive algorithm that:
Finds an empty cell
Tries digits 1-9
Checks if digit is valid (row, column, 3×3 subgrid)
Places digit and recursively solves
Backtracks if no valid solution found
Time Complexity: O(9^m) where m is number of empty cells
Space Complexity: O(m) for recursion stack
👥 Team Members
This project was developed as part of Summer Training Program by:
Jahanvi Sharma (12322669)
Gaurav Kumar (12316984)
Karthik (12313614)
🚀 Future Enhancements
[ ] Graphical User Interface (GUI)
[ ] Random puzzle generator
[ ] Difficulty level selector (Easy/Medium/Hard)
[ ] Hint system for manual solving
[ ] Advanced solving heuristics (Naked Pairs, X-Wing)
[ ] Web application deployment
[ ] Mobile app version
📝 License
This project was developed for educational purposes as part of a summer training program.
🤝 Contributing
Feel free to fork this project and submit pull requests for improvements!
📧 Contact
For questions or suggestions, feel free to reach out to the team members.
⭐ If you found this project helpful, please give it a star!