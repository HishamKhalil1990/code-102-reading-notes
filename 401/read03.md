# FileIO & Exceptions
## FileIO
#### python has the ability to handle files, so it can be read and write on file even analyzing raw byte data. a file is a contiguous set of bytes used to store data in a simple way as text file or complictaed as program executable file. however, files are tarnslated in binary later on to be processed by the computer
#### a file consits of three parts:
1. Header
2. Data
3. End of file 
#### for files, paths are required to be accessed. a path is the file location. paths are consits of:
- folder path
- file name
- extension
#### one of the common problem is encoding of the byte data. encoding is a translation from byte data to human readable characters 
#### in python, opening and closeing files are done by:
- `open()` for opening
- `close()` for closing
#### there are three types of file objeect:
1. Text files
2. Buffered binary files
3. Raw binary files
#### once the file is open, some methods can be applyed as:

| method | what it does |
| ------ | ------------ |
| `.read(size=-1)` | This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read. |
| `.readline(size=-1)` | This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read. |
| `.readlines()` | This reads the remaining lines from the file object and returns them as a list. |
| `.write(string)` | This writes the string to the file. |
| `.writelines(seq)` | This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s). |

## Exceptions
#### in python, when error occur the program is terminated. an error can be a syntax error or an exception. for syntax error, it happen when the parser detects an incorrect statement but in exception happen when a correct syntactically code give an error as a result of code excution as a `ZeroDivisionError` when dividing on zero. to throw the exception, `raise` if a condition occured. however to avoid a program crash midway, `AssertionError` can be used. sometimes when exception occurs, a new algorithms should be used instead. to do this `try` and `except` Block is used where the code try to excute the `try` code block and when it failed it excute the `except` code block. for the last method, an `else` clause can be added to be excuted when no excption occurs or `finally` clause can be added to be excuted always at the end 