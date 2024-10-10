# Automatic-generate-password
import java.util.Random;
public class PasswordGenerater{
public static void main(String args[]){
int length=9;
System.out.println(generatePassword(length));
}
static char[] generatePassword(int len){
System.out.println("Generating Password using random ():");
system.out.print("My new password is:");
String capitalChars = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
        String smallChars = "abcdefghijklmnopqrstuvwxyz";
        String numbers = "0123456789";
        String symbols = "!@#$%^&*_=+-/.?<>)";
        String values = capitalChars + smallChars + numbers + symbols;
        Random randomMethod = new Random();
        char[] password = new char[len];
        for (int i = 0; i < len; i++) {
            password[i] = values.charAt(randomMethod.nextInt(values.length()));
        }

        return password;
    }
}

 
