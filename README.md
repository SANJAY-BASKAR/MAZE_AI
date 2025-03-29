
---

# 🏁 Maze Solver  

A Python program that reads a maze from a text file, solves it using depth-first search (DFS) or breadth-first search (BFS), and generates a visual representation of the solution.  

## ✨ Features  
- Reads a maze from a text file.  
- Finds the shortest path from start (`A`) to goal (`B`).  
- Supports **DFS (StackFrontier)** and **BFS (QueueFrontier)**.  
- Displays the maze and its solution in the terminal.  
- Generates a **visual output (`maze.png`)** with color-coded paths.  

## 📜 How It Works  
1. The program reads a text file containing the maze.  
2. It validates that there is exactly **one start (`A`)** and **one goal (`B`)**.  
3. The solver explores possible paths using a **frontier-based search algorithm**.  
4. The final solution is printed in the terminal and saved as an image.  

## 📌 Installation  
Ensure you have **Python 3** installed. Then, install the required dependency:  
```sh
pip install pillow
```

## 🚀 Usage  
Run the program by providing a maze file as an argument:  
```sh
python maze.py maze1.txt
```
This will:  
✔ Display the maze.  
✔ Solve it and show the explored states.  
✔ Print the solution.  
✔ Save the **solved maze image** (`maze.png`).  

## 📝 Maze Format  
Each maze should be a `.txt` file containing:  
- `#` for **walls**  
- `A` for **start position**  
- `B` for **goal**  
- A space (` `) for **open paths**  

**Example (`maze1.txt`):**  
```
####B#
#### #
####  #
#### ##
     ##
A######
```

## 🎨 Visual Output  
The program generates a **PNG image** (`maze.png`) where:  
🟥 **Red** = Start (`A`)  
🟩 **Green** = Goal (`B`)  
🟨 **Yellow** = Solution Path  
⬛ **Gray** = Walls  

## 🛠 Code Structure  
- **`maze.py`** – Core logic to read, solve, and visualize the maze  
- **`Node` class** – Represents each state in the search tree  
- **`StackFrontier`** & **`QueueFrontier`** – Used for DFS/BFS traversal  

## 🎯 Future Enhancements  
✅ Add more solving algorithms (e.g., A* Search)  
✅ Allow user to choose between DFS/BFS  
✅ Generate random mazes  

## 📷 Example Output  
After running `python maze.py maze1.txt`, the output will look like:  
```
Maze:
####B#
####*#
####**
######
****##
A######
```
And the **maze.png** file will visually display the solution.  

## 📜 License  
This project is **MIT Licensed** – feel free to modify and distribute it!  

---

