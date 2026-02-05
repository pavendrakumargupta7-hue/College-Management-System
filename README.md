# College-Management-System
class College:
    def __init__(self):
        self.menu()

    def menu(self):
        while True:
            choice = int(input("""
1. Press 1 to visit college campus
2. Press 2 to take admission
3. Press 3 to check library
4. Press 4 to check package
5. Press 5 to see course branch
6. Press 6 to see study resources
7. Press 7 to remove admission
8. Press any other key to exit
Enter your choice: 
"""))

            if choice == 1:
                self.visit_college_campus()
            elif choice == 2:
                self.take_admission()
            elif choice == 3:
                self.library()
            elif choice == 4:
                self.check_packages()
            elif choice == 5:
                self.course_branch()
            elif choice == 6:
                self.study_resources()
            elif choice == 7:
                self.remove_admission()
            else:
                print("Thank you! Exiting...")
                break

    def visit_college_campus(self):
        print("""
College Ground Available
College Garden Available
Two Buildings: Technology & Engineering
Two Libraries Available
College Timing: 9:00 AM to 4:00 PM
Bus Facility Available
For more info, contact college faculty.
""")

    def take_admission(self):
        print("Please fill the admission form:")
        name = input("Enter student name: ")
        father_name = input("Enter father name: ")
        mother_name = input("Enter mother name: ")
        aadhar = input("Enter Aadhar number: ")
        print("Submit documents and photos.")
        print("Admission Successful!")

    def library(self):
        print("Library has books, journals, and digital resources.")

    def check_packages(self):
        print("Average package: 4 LPA")

    def course_branch(self):
        print("Courses: CSE, AIML, ECE, ME, CE")

    def study_resources(self):
        print("Notes, PDFs, Online portals available")

    def remove_admission(self):
        print("Admission removed successfully")


# Object creation
college = College()
