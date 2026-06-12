# Linux Day 03

## Objective

Learn basic commands for searching and inspecting files in Linux.

## Commands Learned

### grep
Search for specific text inside files.

Example:
grep "failed" logs.txt

### find
Search for files and directories.

Example:
find . -name "*.txt"

### head
Display the first lines of a file.

Example:
head -5 logs.txt

### tail
Display the last lines of a file.

Example:
tail -5 logs.txt

### less
View file contents page by page.

Example:
less logs.txt

## Practice

- Created sample log files.
- Searched log entries using grep.
- Located files using find.
- Viewed the beginning and end of files using head and tail.
- Navigated file contents using less.

## Notes

- grep is useful for log analysis and searching specific events.
- find helps locate files efficiently.
- head and tail are commonly used when working with large log files.
- less is useful for reading long files without opening an editor.
