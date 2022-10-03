# Visual Studio

Installations is simple. Just download the installer from [here](https://visualstudio.microsoft.com/downloads/).

---

> **Visual C++ Compiler stdc++=20**

## Installation guide

~ Install Visual Sudio

~ Modify Installation

~ Individual Components > search ``` modules ```

## Activation

* Solution Properties > Configuration Properties > General: C++ Language Standard = "Preview - Features from the Latest C++ Working Draft (/std:c++latest)"

* Solution Properties > C/C++ > Language : Enable External C++ Standard Library Modules = "Yes(/experimental:module)"

## **import commands**

* std.filesystem -> `<filesystem>`
* std.regex -> `<regex>`
* std.memory -> `<memory>`
* std.threading -> `<atomic>, <condition_variable>, <future>, <mutex>, <shared_mutex> and <thread>`
* std.core -> Everything else in the Standard Library

> Note: -> = Provides the contents of headers
