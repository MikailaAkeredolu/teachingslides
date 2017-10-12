# teachingslides
class Student extends Person{
    public subjects: string[];  //unique student
    constructor(firstName: string, lastName: string, age: number,  _ssn: string,subjects: string[]){
        super(firstName, lastName, age, _ssn); //prevent this.firtname
        this.subjects = subjects; //new to the Student class
    }
    public printInfo(): void{
         //super.printInfo(); //parent print info method
       console.log('Fullname of student is ' + this.firtName + ' ' + this.lastName + ' and he is learning' + this.subjects);  //overrriding 
    }
}
let student1: Student = new Student('Jose','Perez', 30, '2445', ['Java', 'TypeScript']);
//student1._ssn = '0726';
//student1.ssn = '1326';
// student1.age = 31;
student1.printInfo();
