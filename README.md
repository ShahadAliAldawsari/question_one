# question_one
public class Employee{
    
    String name;
    String position;
    double salary;
    double experience;
    String educational_level;
    double bonus;
    
    public double calculatSalary (double basicSalary){
        double Salary = basicSalary + (basicSalary * 0.05 * Experience)
        if(Educational_level.equals("Bachelor Degree"))
            Salary += 500;
        else if (Educational_level.equals("Diploma"))
            Salary += 250;
        this.salary = Salary;
        return Salary;
    }


}

public class FullTtimeEmployee extends Employee{
    public double calculatBonus (double basicSalary)
        this.bonus = basicSalary*0.03;
        return bonus;
}

public class PartTtimeEmployee extends Employee{
    public double calculatBonus (double basicSalary)
        this.bonus = basicSalary*0.015;
        return bonus;
}
