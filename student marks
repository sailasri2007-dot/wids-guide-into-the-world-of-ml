students = []
marks = {}

def add_student():
    name = input("Enter student name to add: ")
    score = int(input("Enter marks: "))
    students.append(name)
    marks[name] = score
    print(name, "added successfully!\n")

def delete_student():
    name = input("Enter student name to delete: ")
    if name in students:
        students.remove(name)
        del marks[name]
        print(name, "removed successfully!\n")
    else:
        print("Student not found!\n")

def show_students():
    if len(students) == 0:
        print("No students available.\n")
        return 
    
    else:
        print("\nStudent Marks:")
        for name in students:
           print(name, "->", marks[name])

def find_topper():
    if len(marks) == 0:
        print("No students available.\n")
        return
    
    max_marks = -1
    topper = ""

    for name in marks:
        if marks[name] > max_marks:
            max_marks = marks[name]
            topper = name

    print("Topper:", topper, "with marks", max_marks, "\n")

while True:
    print("1. Add Student")
    print("2. Delete Student")
    print("3. Show Students")
    print("4. Find Topper")
    print("5. Exit")

    choice = input("Enter your choice: ")

    if choice == "1":
        add_student()
    elif choice == "2":
        delete_student()
    elif choice == "3":
        show_students()
    elif choice == "4":
        find_topper()
    elif choice == "5":
        print("Program Ended.")
        break
    else:
        print("Invalid choice!\n")
