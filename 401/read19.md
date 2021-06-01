# Automation
## Regular Expressions
### Regular Expressions (regex) are a sequence of characters used to check whether a pattern exists in a given text string or not. They can be used to validate the format of email addresses or passwords. in python, `re` is a Python library that supports regular expressions.
### `re` library provide methods such as: 
- `match()` function returns a match object if the text matches the pattern. Otherwise, it returns None. ex; `re.match(pattern, sequence)`
- `compile()` turn a regular expression pattern into a regular expression object. ex; `pattern = re.compile(r"cookie")` rhen to search for this regex we use `pattern.search(sequence).group()`
- `search()` scan through the given string/sequence, looking for the first location where the regular expression produces a match and with `group()` it returns the string matched by the `re`. ex; `re.search(r'Co.k.e', 'Cookie').group()`
- `findall()` finds all the possible matches in the entire sequence but returns regex match objects as an iterator. ex; `re.findall(pattern, statement)` 
- `sub()` substitute function. It returns the string obtained by replacing or substituting the leftmost non-overlapping occurrences of pattern in string. ex; `re.sub(r'([\w\.-]+)', r'support@datacamp.com', statement)`
- `split()` splits the strings wherever the pattern matches and returns a list. ex; `pattern.split(statement)`
## shutil
### shutil module includes high-level file operations such:
- copying:
    - **Copying Files** using `copyfile()`, it copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file
    - **Copying Files** using `copy()`, it interprets the output name like the Unix command line tool cp
    - **Copying File Metadata** using `copymode()`, it copys the permissions from one file to another
    - **Copying Directory Trees** using `copytree()`, it copys a directory from one place to another and recurses through the source directory tree, copying files to the destination
- Finding:
    - **Finding Files** using `which()`, it scans a search path looking for a named file to find an executable program on the shell’s search path defined in the environment variable PATH
- archiving:
    - **Archive Files** using `get_archive_formats()`, it returns a sequence of names and descriptions for formats supported on the current system
    - **Create Archive** using `make_archive()`, it creates a new archive file
    - **Extract Archive** using `unpack_archive()`, it extracts the archive by passing the archive file name and optionally the directory where it should be extracted
- File System Space:
    - **File System Space** using `disk_usage()`, it is useful to examine the local file system to see how much space is available before performing a long running operation and it returns a tuple with the total space, the amount currently being used, and the amount remaining free