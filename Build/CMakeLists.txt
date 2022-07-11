cmake_minimum_required(VERSION 2.8.9)
set(CMAKE_CXX_STANDARD 11)
project (EquinoxLoggerDemo)
add_library(EquinoxCLogger STATIC 

#interfaces
../Source/EquinoxLogger/IFile-Logger.h
../Source/EquinoxLogger/IConsole-Logger.h
../Source/EquinoxLogger/ILogger-Level.h
../Source/EquinoxLogger/ILogger-Output.h
../Source/EquinoxLogger/ILogger-Time.h

#headers
../Source/EquinoxLogger/Logger.h
../Source/EquinoxLogger/Log-Level-Type.h
../Source/EquinoxLogger/Log-Output-Type.h
../Source/EquinoxLogger/File-Logger.h
../Source/EquinoxLogger/Console-Logger.h
../Source/EquinoxLogger/Logger-Level.h
../Source/EquinoxLogger/Logger-Output.h
../Source/EquinoxLogger/Logger-Time.h

#source
../Source/EquinoxLogger/Logger.cpp
../Source/EquinoxLogger/File-Logger.cpp
../Source/EquinoxLogger/Console-Logger.cpp
../Source/EquinoxLogger/Logger-Level.cpp
../Source/EquinoxLogger/Logger-Output.cpp
../Source/EquinoxLogger/Logger-Time.cpp
)
