#include <stdio.h>

// Structure to hold student information
struct Student {
    char name[50];
    int rollNumber;
    float marks;
    char grade;
};

// Function to add student data
void addStudent(struct Student students[], int index) {
    printf("Enter details for student %d:\n", index + 1);
    printf("Name: ");
    scanf("%s", students[index].name);
    printf("Roll Number: ");
    scanf("%d", &students[index].rollNumber);
    printf("Marks: ");
    scanf("%f", &students[index].marks);

    // Calculate grade based on marks
    if (students[index].marks >= 90)
        students[index].grade = 'A';
    else if (students[index].marks >= 80)
        students[index].grade = 'B';
    else if (students[index].marks >= 70)
        students[index].grade = 'C';
    else if (students[index].marks >= 60)
        students[index].grade = 'D';
    else
        students[index].grade = 'F';

    printf("Student added successfully!\n\n");
}

// Function to display student data
void displayStudents(struct Student students[], int count) {
    printf("Student Data:\n");
    for (int i = 0; i < count; i++) {
        printf("Student %d\n", i + 1);
        printf("Name: %s\n", students[i].name);
        printf("Roll Number: %d\n", students[i].rollNumber);
        printf("Marks: %.2f\n", students[i].marks);
        printf("Grade: %c\n\n", students[i].grade);
    }
}

int main() {
    int numStudents;
    printf("Enter the number of students: ");
    scanf("%d", &numStudents);

    // Create an array of structures to hold student data
    struct Student students[numStudents];

    // Add student data
    for (int i = 0; i < numStudents; i++) {
        addStudent(students, i);
    }

    // Display student data
    displayStudents(students, numStudents);

    return 0;
}
