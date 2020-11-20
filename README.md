# Tool-Lib v1.2

# Introduction

Tool-Lib is a small library used to make Simple Batch Plugins without writing more code for every C functions.

# How to use Tool-Lib?

To use Tool-Lib you need to know basics of C Programming Language to implement the functions in your program. If you are familiar with C then just download it from GitHub and include header files by config.h. After adding just open .c files in any code editor and see the functions which I use the library and copy the functions, after this just put it on your code and compile it using GCC or TCC. After compilation you will found a executable file, just run and enjoy!

# How much functions stay in this library?

There are some basic functions and some maths there, it's not very big library it just used to make Simple Batch Plugins. You can use it for your purpose.

The Functions which are stay on it:

In winapi.c

tool_gotoxy(int x and int y); // Change cursor position on cmd by X and Y value.
tool_cursor_state(int state); // Change cursor state (0 = ShowCursor) else (1 = HideCursor)
tool_tool_clear_screen();// Clear the whole console screen like CLS command. (** In old version I used Dos9 Clear function but in this version I use my own function)
tool_change_color(char color); // Change console color (** Only arguments in char, if you try to give integers you will found warning in compilation)
tool_default_color(); // Same as color 07 or color 7
tool_cursor_size(int size); // Change cursor size of blinking cursor
tool_get_time(); // To get system local time (** If your local time is wrong then you will find the wrong time)
tool_millisleep(int sleep); // Wait for milliseconds
tool_secondsleep(int sleep); // Wait for seconds
tool_buffer_size(int x, int y); // Set cmd buffer size
tool_flush_console(); // Flush the whole cmd

End of winapi.c

So you can see some functions here in it you will find more, here is not posible to give every functions, to know just visit the source.

# Why TCC gives error to compile some libs?

Compiler is a important question to everyone, in include of TCC there are many functions were removed for the reason you getting this errors. To solve the issue use MinGW or TDM-GCC or DevC++. To download TDM-GCC just follow the link. https://sourceforge.net/projects/tdm-gcc/

# Why MinGW gives warnings and errors?

Actually I made it based on TDM-GCC, because it's much better and most of programs (Ex: LZMA) is compiled under this compiler so I recomended use TDM-GCC, to download follow the link which I provide.

# Is modification allowed?

Yes, you can use the functions in your program or modify the functions as you want under MIT License.

# What is the next step of Tool-Lib?

I want to make a DLL (Dynamic Link Library) of Tool-Lib which contains every functions as Tool-Lib contains. Benefits happed that you just need to load a DLL in memory don't need to add library.

# About

This program under MIT License.
Copyright (C) 2018-2020 MathInDOS

