# COA_Docker
# Python YAML Use Case - Student Information Management

## Overview
This Python application reads student data from a YAML file and provides options to display and filter the data based on GPA. It demonstrates how to handle YAML files in Python using the PyYAML library.

## Features
- Reads student information from a `students.yaml` file.
- Displays all students with their details.
- Filters and displays students based on a minimum GPA input.

## Installation
Ensure you have Python installed. Then, install the required package:
```sh
pip install pyyaml
```

## Project Structure
```
project_directory/
│── app.py          # Python script to run the application
│── students.yaml   # YAML file containing student data
│── README.md       # Project documentation
```

## YAML File Format (`students.yaml`)
```yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
  - name: Bob
    age: 22
    major: Mathematics
    gpa: 3.5
  - name: Charlie
    age: 20
    major: Physics
    gpa: 3.9
  - name: David
    age: 23
    major: Chemistry
    gpa: 3.2
  - name: Eva
    age: 21
    major: Computer Science
    gpa: 3.7
```

## How to Run the Application
1. Ensure `app.py` and `students.yaml` are in the same directory.
2. Open a terminal and navigate to the directory.
3. Run the script using:
   ```sh
   python app.py
   ```
4. The application will display all students and prompt you to enter a minimum GPA to filter students.

## Expected Output
```
All Students:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Bob, Age: 22, Major: Mathematics, GPA: 3.5
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: David, Age: 23, Major: Chemistry, GPA: 3.2
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7

Enter minimum GPA to filter students: 3.6
Students with GPA >= 3.6:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7
```

## Code Explanation
- **Loading Data:** The `load_data` function reads the YAML file and converts it into a Python dictionary.
- **Displaying Students:** The `display_students` function prints all student details.
- **Filtering Students:** The `filter_students_by_gpa` function filters students based on the provided minimum GPA.
- **Main Execution:** The `main` function orchestrates the process and prompts user input.

## Future Enhancements
- Add functionality to update and save student data.
- Implement sorting options.
- Convert the script into a graphical user interface (GUI) application.

## License
This project is open-source and free to use for educational purposes.

---
This README file provides a clear understanding of the project, setup instructions, and usage guidelines.

