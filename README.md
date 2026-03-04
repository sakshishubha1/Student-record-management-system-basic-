# Student Record Management System

A simple C program that manages student records with persistent file storage.

## Features

- **Add Student Records**: Add new student information (name, roll number, marks) to the system
- **View All Records**: Display all stored student records
- **Search by Roll Number**: Find and display specific student records by their roll number
- **Persistent Storage**: All records are saved to a file for data persistence

## Project Structure

- `studentrecordproject.c` - Main program file containing all functionality

## Data Storage

Student records are stored in a text file named `prant.txt` with the following format:
```
name roll_number marks
```

## Usage

### Compilation

```bash
gcc studentrecordproject.c -o studentrecordproject
```

### Running the Program

```bash
./studentrecordproject
```

### Menu Options

The program presents an interactive menu with the following options:

1. **Add Student Records** - Enter student details (name, roll number, marks)
2. **View All Records** - Display all stored student records
3. **Search by Roll Number** - Search for a specific student using their roll number
4. **Exit** - Quit the program

## Data Structure

The program uses a `Student` structure to store:
- `name` (character array, max 100 characters)
- `roll` (integer - roll number)
- `marks` (integer - student marks)

## Example Output

```
Enter 1 to add students record, enter 2 to view all student records, enter 3 to search student through roll number, 4 to exit: 1
How many records do you want to add? 2
Enter data for 1 student name, roll number, marks: John 101 85
Enter data for 2 student name, roll number, marks: Jane 102 92
```

## Requirements

- C compiler (gcc, clang, or similar)
- Standard C library
- Read/write permissions in the working directory

## Notes

- Records are appended to the file, so existing data is preserved when adding new records
- The program creates the `prant.txt` file automatically if it doesn't exist
- Search is case-sensitive for names
