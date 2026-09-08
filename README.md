# CDataframe

A C library that provides a DataFrame-like data structure and operations, inspired by Python's Pandas library.

## Description

Spreadsheet applications such as LibreOffice Calc and Microsoft Excel can be used to store, display, sort, and manipulate tabular data.

In Python, the [Pandas](https://pandas.pydata.org/) library provides a powerful `DataFrame` structure for importing, cleaning, analysing, manipulating, and visualising data.

The C language does not provide an equivalent data structure by default. The goal of **CDataframe** is to provide a C-based alternative that implements a selection of DataFrame operations inspired by Pandas.

The project uses dynamic arrays to store and manipulate data and provides an interactive program through which the different operations can be tested.

The repository contains two main versions:

* **`main`** — the most advanced version, supporting the full CDataframe implementation.
* **`part_one`** — an earlier prototype that only supports integer values.

## Getting Started

### Dependencies

To compile and run the project, you need:

* A C compiler such as **GCC**
* A terminal or command prompt
* A C development environment such as **Visual Studio Code**, **Code::Blocks**, or **CLion** (optional)

The project is designed to run on common operating systems such as Windows, Linux, and macOS, provided a compatible C compiler is available.

### Installing

Clone the main version of the project:

```bash
git clone https://github.com/hezaqqq/cdataframe.git
```

To clone the `part_one` prototype instead:

```bash
git clone -b part_one https://github.com/hezaqqq/cdataframe.git
```

Then navigate to the project directory:

```bash
cd cdataframe
```

Alternatively, you can download the project directly from the [GitHub repository](https://github.com/hezaqqq/CDataframe_tacca_tran).

Make sure that `main.c` is located in the same directory as the other `.c` and `.h` files.

### Executing program

Compile the project using your C compiler. For example, with GCC:

```bash
gcc *.c -o cdataframe
```

Then run the program:

**Linux / macOS:**

```bash
./cdataframe
```

**Windows:**

```bash
cdataframe.exe
```

Once the program starts, an interactive menu will be displayed.

1. Create a CDataframe by selecting command **1**.
2. Select the command corresponding to the operation you want to perform.
3. Follow the instructions displayed by the program.
4. Use the available commands to manipulate and inspect the CDataframe.

## Help

### The program does not compile

Make sure that:

* All `.c` and `.h` files are present in the project directory.
* `main.c` is located alongside the other source files.
* Your C compiler is correctly installed and accessible from the terminal.

For GCC, you can check your installation with:

```bash
gcc --version
```

### The program does not start

Make sure you are running the executable from the correct directory.

On Linux/macOS:

```bash
./cdataframe
```

On Windows:

```bash
cdataframe.exe
```

### Testing individual functions

Some functions are not included in the interactive menu because they are intended to be used internally by other CDataframe functions.

To test these functions directly, modify `main.c` and call the desired function manually.
