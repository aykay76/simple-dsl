I was looking on my bookshelf and saw 'Writing Compilers and Interpreters, An applied approach using C++' by Donald Mak.

I bought the book and followed the code initially to create a 3D modelling language which was used to drive a 3D plugin for web browsers (this was 2005 so it was Flash, Silverlight or nothing at that point).

Now i'm looking to create simple DSLs for different purposes, so thought it would be fun to brush off this code and convert it to C# so that I can use it in a .NET core application.

This code represents the first few chapters of the book that guide you through creating a stream tokeniser, parser and rudimentary interpreter. It deals with basic concepts like variables and a runtime stack. It does not support functions and flow control.

I have now finished the code for the rest of the book and have a working Pascal interpreter that includes functions, procedures and if/while/repeat/for flow control blocks.

As part of the move to C# I had to refactor some pointer arithmetic and masking of different types behind void pointers. I have also tried to abstract out the Pascal specific constructs so that I can reuse the base scanner, parser and type system to create additional DSLs.
