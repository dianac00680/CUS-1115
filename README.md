# 🎲 Java Random Array

This simple Java program creates a double array with 1000 cells, fills it with random values between 1.0 and 207.56, and prints the contents to the console.

## 💡 Features
- Fills array with random values
- Clean and simple structure
- Beginner-friendly Java syntax

## 🛠 How to Run

Compile and run using:

```bash
javac RandomArray.java
java RandomArray


---

### 👨‍💻 `RandomArray.java`

```java
import java.util.Random;

public class RandomArray {
    public static void main(String[] args) {
        double[] array = new double[1000];
        Random rand = new Random();

        for (int i = 0; i < array.length; i++) {
            array[i] = 1.0 + (207.56 - 1.0) * rand.nextDouble();
        }

        for (double value : array) {
            System.out.printf("%.2f ", value);
        }
    }
}
