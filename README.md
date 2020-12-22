# SumCalculatorChallenge
package academy.learnprogrmming;

public class SimpleCalculator {
    public double firstNumber;
    public double secondNumber;


    public void setFirstNumber(double firstNumber){

        this.firstNumber = firstNumber;
    }
    public double getFirstNumber() {
        return firstNumber;
    }
    public void setSecondNumber(double secondNumber){
        this.secondNumber = secondNumber;

    }

    public double getSecondNumber() {
        return secondNumber;
    }

    public double getAdditionResult(){
        return firstNumber + secondNumber;
    }
    public double getSubtractionResult(){
        return secondNumber - firstNumber;
    }
    public double getMultiplicationResult(){
        return firstNumber * secondNumber;
    }
    public double getDivisionResult(){
        if(secondNumber == 0) {
            return 0;
        }
        return firstNumber / secondNumber;

    }
}
package academy.learnprogrmming;

public class Main {

    public static void main(String[] args) {

        SimpleCalculator calculator = new SimpleCalculator();
        calculator.getFirstNumber();
        calculator.setFirstNumber(5.0);
        calculator.getSecondNumber();
        calculator.setSecondNumber(4);
        System.out.println("Add= " + calculator.getAdditionResult());
        System.out.println("Subtract= " + calculator.getSubtractionResult());
        calculator.setFirstNumber(5.25);
        calculator.setSecondNumber(0);
        System.out.println("multiply= " + calculator.getMultiplicationResult());
        System.out.println("divide= " + calculator.getDivisionResult());
    }
}
