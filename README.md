# question_one
public class Employee {

    String name;
    String position;
    double salary;
    double experience;
    String educational_level;
    double bonus;

    Employee(String name, String position, double experience, String educational_level) {
        this.name = name;
        this.position = position;
        this.experience = experience;
        this.educational_level = educational_level;
    }

    public double calculatSalary(double basicSalary) {
        double Salary = basicSalary + (basicSalary * 0.05 * experience);
        if (educational_level.equals("Bachelor Degree"))
            Salary += 500;
        else if (educational_level.equals("Diploma"))
            Salary += 250;
        this.salary = Salary;
        return Salary;
    }

}

class FullTtimeEmployee extends Employee {
    FullTtimeEmployee(String name, String position, double experience, String educational_level) {
        super(name, position, experience, educational_level);
    }

    public double calculatBonus(double basicSalary) {
        this.bonus = basicSalary * 0.03;
        return bonus;
    }
}

class PartTtimeEmployee extends Employee {
    PartTtimeEmployee(String name, String position, double experience, String educational_level) {
        super(name, position, experience, educational_level);
    }

    public double calculatBonus(double basicSalary) {
        this.bonus = basicSalary * 0.015;
        return bonus;
    }
}
