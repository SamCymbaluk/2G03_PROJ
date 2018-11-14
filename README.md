# CNN
C NeuralNets: A simple neural network library in C

### Installation
```bash
git clone https://github.com/SamCymbaluk/CNN.git
cd CNN
make build
```
This will create a `cnn.so` shared object file in the CNN directory beside the cnn.h header file.

You can use this in your own C program like so:
```C
#include "path/to/cnn.h"

int main() {
  ...
};
```
And compile with
```bash
gcc -c myprog.c
gcc -o myprog myprog.o -Lpath/to/cnn.so -l:cnn.so
```

### Demos
This repo includes a number of demos to play with.
Compile the demos by running `make demos`.
You can then try them out by executing one of the following commands in the CNN directory:
```bash
./xor_demo
./mnist_demo
```
