Multithread Sobel filter implementation on C language.

## About
1. Working only with `PGM - portable graymap format` image
2. Support multithreading using `-J` flag

## Flags
- `-S` Path to source PGM image `required!`
- `-O` Path to output PGM image `required!`
- `-J` Threads count `optional`

## Usage
```bash
git clone https://github.com/DieTime/sobel-filter.git
cd sobel-filter/

cmake -DCMAKE_BUILD_TYPE=Release -S . -B ./cmake-build
cd ./cmake-build && cmake --build . --config Release

./sobel-filter -S <path/to/source.pgm> -O <path/to/output.pgm> -J <threads>
```
