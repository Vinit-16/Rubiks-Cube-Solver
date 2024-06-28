cmake_minimum_required(VERSION 3.28)
project(Rubiks_Cube_Solver)

set(CMAKE_CXX_STANDARD 17)

add_executable(Rubiks_Cube_Solver main.cpp
        PatternDatabases/PatternDatabase.h
        PatternDatabases/PatternDatabase.cpp
        PatternDatabases/NibbleArray.h
        PatternDatabases/NibbleArray.cpp
        PatternDatabases/math.cpp
        PatternDatabases/math.h
        PatternDatabases/CornerPatternDatabase.cpp
        PatternDatabases/CornerPatternDatabase.h
        PatternDatabases/CornerDBMaker.cpp
        PatternDatabases/CornerDBMaker.h
        PatternDatabases/PermutationIndexer.h
        Model/RubiksCube.cpp
        Model/RubiksCube.h
        Model/RubiksCube1dArray.cpp
        Model/RubiksCube3dArray.cpp
        Model/RubiksCubeBitboard.cpp
        Model/PatternDatabase/PatternDatabase.h
        Solver/BFSSolver.h
        Solver/DFSSolver.h
        Solver/IDAstarSolver.h
        Solver/IDDFSSolver.h)
