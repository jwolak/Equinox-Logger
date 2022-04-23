# Equinox logging engine
**Thread safety C++ logger with C-style MACRO interface**

***To version written in C, please visit: https://github.com/jwolak/EquinoxC-Logger***


**Logger with support logging to file, console or both. Four levels avaliable:**
- Error 
- Warning
- Debug
- Disabled

## Features

- settable log level
- settable output direction (console, file or both)
- interface as enjoyable C-style macros
- powered by C++11


## Building for source

###### For EquinoxLoggerDemo:

```sh
cd Build/
cmake CMakeLists.txt
make
```

###### For UnitTests:

```sh
cd UnitTests/Build
cmake CMakeLists.txt
make
```
## Example:

Include "EquinoxLogger/Logger.h" to your source code:
```sh
See: Source/main.cpp
```
```sh
#include "EquinoxLogger/Logger.h"

int main(void) {

  SET_LOG_LEVEL(equinox_logger::LogLevelType::LOG_LEVEL_DEBUG);
  SET_LOG_LOGGER_OUTPUT(equinox_logger::LogOutputType::FILE_AND_CONSOLE);

  LOG_ERROR("%s", "Test log");
  LOG_WARNING("%s %d %f", "Values: ", 4, 3.5f);
  LOG_DEBUG("Debug text: %f %s", 4.5, "post debug text");

  return 0;
}
```
## License

BSD 3-Clause License

***Copyright (c) 2022, Janusz Wolak***

All rights reserved.

