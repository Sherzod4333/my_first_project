# my_first_project
public class Car {
    // 🔒 1. Private o'zgaruvchilar (Encapsulation)
    private String model;
    private String color;
    private double price;
    private boolean isAutomatic;

    // 🚗 2. Konstruktor
    public Car(String model, String color, double price, boolean isAutomatic) {
        this.model = model;
        this.color = color;
        this.price = price;
        this.isAutomatic = isAutomatic;
    }

    // 🧰 3. Getter va Setter metodlar
    public String getModel() {
        return model;
    }

    public void setModel(String model) {
        this.model = model;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public double getPrice() {
        return price;
    }

    public void setPrice(double price) {
        if (price > 0) {
            this.price = price;
        } else {
            System.out.println("Narx musbat bo‘lishi kerak!");
        }
    }

    public boolean isAutomatic() {
        return isAutomatic;
    }

    public void setAutomatic(boolean automatic) {
        isAutomatic = automatic;
    }

    // 🗣️ 4. Ma'lumot chiqaruvchi metod
    public void displayInfo() {
        System.out.println("🚘 Mashina haqida ma'lumot:");
        System.out.println("Model: " + model);
        System.out.println("Rang: " + color);
        System.out.println("Narx: $" + price);
        System.out.println("Tizimi: " + (isAutomatic ? "Avtomat" : "Mexanik"));
    }
}
