# Projects
package com.company;
import java.util.Scanner;
import java.util.Random;

public class pratixset_2 {
    public static void main(String[] args) {
        //0 for Rock
        //1 for Paper
        //2 for Seasor

        Scanner sc = new Scanner(System.in);
        System.out.println("Enter 0 for Rock , 1 for Paper , 2 for Seasor");
        int userInput = sc.nextInt();

        Random random = new Random();
        int computerInput = random.nextInt();

        if (userInput == computerInput) {
            System.out.println("Draw");
        }
        else if (userInput == 0 && computerInput == 2 || userInput ==1 && computerInput == 0 || userInput ==2 && computerInput == 1){
            System.out.println("You Win");
        }
        else {
            System.out.println("You are Lost.... better Luck Next Time.....!!!!!!");
        }
        System.out.println("Computer Choice" + computerInput);
    }
}
