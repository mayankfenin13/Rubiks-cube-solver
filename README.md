Rubik's Cube Solver ✨

A powerful and flexible C++ Rubik's Cube Solver implementing a variety of search algorithms including:

Depth-First Search (DFS)

Breadth-First Search (BFS)

Iterative Deepening DFS (IDDFS)

Iterative Deepening A* (IDA*) with a Corner Pattern Database

Built for speed ⚡ and understanding of classic AI algorithms applied to a 3D puzzle.

📚 Features

Multiple cube representations:

3D Array-based Cube

1D Array-based Cube

Bitboard-based Cube (extremely fast)

Modular solver classes

Pattern Database support for optimized solving

Cross-platform CMake support

CLI-based visualization of cube state and move history

🛠️ Installation & Build

1. Clone the repository

git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO

2. Install CMake (if not installed)

brew install cmake     # for macOS
sudo apt install cmake # for Linux

3. Build the project

mkdir build
cd build
cmake ..
make

4. Run the solver

./rubiks_cube_solver

🔧 Usage

By default, the program will:

Generate a random shuffle of a Rubik's Cube

Solve it using the IDA* algorithm

Display the cube before and after

Print the moves required to solve it

🔎 Example Output

Rubik's Cube:

G Y B
Y W W
Y Y O
...

Shuffle moves:
D' F' D R' U' D2 L U' F2 R2 B' B' R2

Solved Cube:
...

Solution moves:
F R U D2 ...

📑 File Structure

.
├── Model/
│   ├── RubiksCube.h / .cpp
│   ├── RubiksCube3dArray.cpp
│   ├── RubiksCube1dArray.cpp
│   └── RubiksCubeBitboard.cpp
├── Solver/
│   ├── DFSSolver.h
│   ├── BFSSolver.h
│   ├── IDDFSSolver.h
│   └── IDAstarSolver.h
├── PatternDatabases/
│   ├── CornerDBMaker.h / .cpp
│   ├── CornerPatternDatabase.h / .cpp
│   └── utils: NibbleArray, math, PermutationIndexer
├── main.cpp
└── CMakeLists.txt

📦 Corner Pattern Database

To generate the database:

CornerDBMaker dbMaker("Databases/cornerDepth5V1.txt", 0x99);
dbMaker.bfsAndStore();

To use the pre-generated database:

IDAstarSolver<RubiksCubeBitboard, HashBitboard> idaStarSolver(cube, "Databases/cornerDepth5V1.txt");
auto moves = idaStarSolver.solve();

🚀 Future Improvements

Facelet color input parser

GUI using OpenGL or SDL

Full edge + corner pattern database

Parallelized solver

👨‍💼 Author

Mayank FeninBuilt as a passion project to learn algorithms, C++, and the beauty of the cube!

✨ Star the Repo

If this project helped you or inspired you:

git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO

Then feel free to ⭐ star it on GitHub!

📥 License

This project is open-sourced under the MIT License.

🙌 Acknowledgments

Inspired by the beauty and challenge of the Rubik’s Cube 🟩🟥🟦

Thanks to all the tutorials and contributors in the C++ open-source community!

