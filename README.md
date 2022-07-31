# Java-Basics-at-SoftUni
Java Basics at SoftUni


////

import java.util.Scanner;

class Car {
    private String brand;
    private String model;
    private int horsePower;

    public Car(String brand, String model, int horsePower) {
        this.brand = brand;
        this.model = model;
        this.horsePower = horsePower;
    }

    public String getBrand() {
        return brand;
    }

    public String getModel() {
        return model;
    }

    public int getHorsePower() {
        return horsePower;
    }

    @Override
    public String toString() {
        return String.format("%s:%s:%d", this.getBrand(), this.getModel(), this.getHorsePower());
    }
}


public class Main {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        String brand = scanner.nextLine();
        String model = scanner.nextLine();
        int horsePower = Integer.parseInt(scanner.nextLine());

        Car car = new Car(brand, model, horsePower);

        System.out.println(car);
    }
}
