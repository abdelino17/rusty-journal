# Rusty Journal

A command-line program to manage to-do list items in rust.

This project is the final program of the [Microsoft Introduction Rust Course](https://docs.microsoft.com/en-gb/learn/paths/rust-first-steps/).

### Features of the program

1. Add new tasks to a to-do list.

2. Remove completed tasks from that list.

3. Print all the current tasks in the list.

### Setup

1. Clone the repo `git clone https://github.com/abdelino17/rusty-journal`

2. Build the application `cd rusty-journal && cargo build`

### Usage

The subcommands available are:

- `add`: Write tasks to the journal file
- `done`: Remove an entry from the journal file by position
- `help`: Prints this message or the help of the given subcommand(s)
- `list`: List all tasks in the journal file

The default journal file is located in the home directory (`~/rusty-journal.json`) but you can change it by specifying the `-j` option.

### Examples

```
$ ./rusty-journal -j test.json add "buy a milk"

$ ./rusty-journal -j test.json add "water the plant"

$ ./rusty-journal -j test.json list

$ ./rusty-journal -j test.json done 2
```
