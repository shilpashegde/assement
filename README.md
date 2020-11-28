# assement
package com.assessment.goodies;

import java.io.*;
import java.util.*;

public class Item {
	String name;
	int price;

	public Item(String name, int price) {
		this.name = name;
		this.price = price;
	}

	public String toString() {
		return this.name + ": " + this.price;
	}
}

class Main {

	public static void main(String[] args) throws Exception {
		FileInputStream fis = new FileInputStream("C:\\Files\\1.html");
		Scanner sc = new Scanner(fis);
		int number_of_employees = Integer.parseInt(sc.nextLine());
		sc.nextLine();

		FileWriter fw = new FileWriter("C:\\Files\\output.htlm");
		fw.write("The goodies selected for distribution are:\n\n");
		

		fw.write("\nAnd the difference between the chosen goodie with highest price and the lowest price is ");
		fw.close();
	}

}
