import java.util.ArrayList;
import java.util.List;

class Student {
    private String name;
    private int age;
    private String faculty;

    public Student(String name, int age, String faculty) {
        this.name = name;
        this.age = age;
        this.faculty = faculty;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        if (age > 0) {
            this.age = age;
        } else {
            System.out.println("Age must be greater than 0");
        }
    }

    public String getFaculty() {
        return faculty;
    }

    public void setFaculty(String faculty) {
        this.faculty = faculty;
    }

    public void printInfo() {
        System.out.println("Name - " + name + ", Age - " + age + ", Faculty - " + faculty);
    }
}

class Teacher {
    private String name;
    private String subject;
    private int expYears;

    public Teacher(String name, String subject, int expYears) {
        this.name = name;
        this.subject = subject;
        this.expYears = expYears;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getSubject() {
        return subject;
    }

    public void setSubject(String subject) {
        this.subject = subject;
    }

    public int getExpYears() {
        return expYears;
    }

    public void setExpYears(int expYears) {
        if (expYears >= 0) {
            this.expYears = expYears;
        } else {
            System.out.println("Experience years must be non-negative");
        }
    }

    public void printInfo() {
        System.out.println("Name - " + name + ", Subject - " + subject + ", Experience Years - " + expYears);
    }
}

class Course {
    private String courseName;
    private Teacher teacher;
    private List<Student> students;

    public Course(String courseName, Teacher teacher) {
        this.courseName = courseName;
        this.teacher = teacher;
        this.students = new ArrayList<>();
    }

    public String getCourseName() {
        return courseName;
    }

    public void setCourseName(String courseName) {
        this.courseName = courseName;
    }

    public Teacher getTeacher() {
        return teacher;
    }

    public void setTeacher(Teacher teacher) {
        this.teacher = teacher;
    }

    public List<Student> getStudents() {
        return students;
    }

    public void addStudent(Student student) {
        students.add(student);
    }

    public void removeStudent(Student student) {
        students.remove(student);
    }

    public void printCourse() {
        System.out.println("Course - " + courseName);
        teacher.printInfo();
        System.out.println("Students:");
        for (Student student : students) {
            student.printInfo();
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Student student1 = new Student("Mark", 18, "Mathematics");
        Student student2 = new Student("John", 20, "Physics");
        Student student3 = new Student("Elena", 19, "Chemistry");

        Teacher teacher1 = new Teacher("Oksana Petrovna", "Biology", 15);
        Teacher teacher2 = new Teacher("Igor Vasilievich", "Programming", 10);

        Course biologyCourse = new Course("Biology Basics", teacher1);
        Course programmingCourse = new Course("Intro to Programming", teacher2);

        biologyCourse.addStudent(student1);
        biologyCourse.addStudent(student3);
        programmingCourse.addStudent(student2);

        biologyCourse.printCourse();
        System.out.println();
        programmingCourse.printCourse();
    }
}
