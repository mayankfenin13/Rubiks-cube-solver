# 🧹 Rubik's Cube Solver

A C++ implementation of a **Rubik’s Cube solver** using object-oriented programming (OOP) principles. This project allows users to simulate, manipulate, and solve a 3×3 Rubik’s Cube directly from the command line.

---

## 🚀 Features

* 🧠 Fully functional cube representation
* 🔁 Supports all basic face rotations (U, D, L, R, F, B)
* 🔄 Supports cube scrambling and resets
* 🛮 Includes a basic solving algorithm (extendable)
* 🛡 Written using clean object-oriented C++ design
* 🗪 Unit-tested components for reliability

---

## 📁 Project Structure

```
Rubiks-cube-solver/
├── include/
│   └── RubiksCube.h          # Cube class declaration
├── src/
│   └── RubiksCube.cpp        # Cube class implementation
├── main.cpp                  # CLI and test interface
├── .gitignore
├── README.md
└── Makefile / CMakeLists.txt (optional)
```

---

## 🚠 Setup Instructions

### ✅ Prerequisites

* C++17 compatible compiler (e.g., g++, clang++)
* Git
* (Optional) `make` or `cmake` if you want to use build systems

---

### 🔃 Clone the Repository

```bash
git clone https://github.com/mayankfenin13/Rubiks-cube-solver.git
cd Rubiks-cube-solver
```

---

### 🛡 Build and Run

#### Option 1: Using `g++` directly

```bash
g++ src/RubiksCube.cpp main.cpp -o cube
./cube
```

#### Option 2: Using `make` (if Makefile exists)

```bash
make
./cube
```

---

## 🔹 Usage

Once you run the executable:

* Use commands like:

  ```
  U  → rotate Up face clockwise
  U' → rotate Up face counterclockwise
  F, R, L, B, D → other face rotations
  scramble → to shuffle the cube
  solve    → to (try to) solve it
  display  → to print the current cube state
  reset    → to restore to solved state
  exit     → to quit the program
  ```

---

## 🧠 Example

```
Welcome to the Rubik’s Cube Solver!

Enter a command:
> scramble
> display
> solve
> display
> exit
```

---

## 🗪 Testing

You can include your own tests in `main.cpp` or write a separate test suite using `Catch2` or `Google Test`.

---

## 🧑‍💻 Contribution

Pull requests are welcome! If you'd like to:

* Add a better solving algorithm (e.g., Kociemba’s algorithm)
* Add GUI or animation
* Improve performance

Feel free to fork and contribute!

---

## 📄 License

This project is open source under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

* Inspired by the beauty and challenge of the Rubik’s Cube 🟩🟥🟦
* Thanks to all the tutorials and contributors in the C++ open-source community!

---
