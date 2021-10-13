## the compiler and pre-processor
```bash
create a new file named mapags.cpp
$ git add mpags.cpp
$ git rm mpags.cpp #delect the file
#g++ compiler
#-std. -This defines waht C++ 'standard' to use.
#-o  -the filename to output to  
$ g++ -std=c++11 -o mpags mpags.cpp
$ ./mpags

# Compiler Eooros and Warnings
#-Wall -Enables some common warnings(NB: not all!)
#-Wextra -Even more warnings
$g++ -Wall -Wextra -std=c++11 -o myprogram main.cpp

```

structrue:
```C
#include<iostream>
#include<string>
int mian()
{
    
}
```
output:
std::cout << my_var << std::endl;

const double a{1};
const int b{2};
std:: sting c{3};

Parameters vs Arguments
Loops(1): for (<initialisation>;<condition>;<loop_process>){<code_block>}