package com.technoelevate.LeapYear;

import java.util.Scanner;

public class Year_n_Month {

	public static void main(String[] args) {
		Scanner scn = new Scanner(System.in);
		System.out.print("Enter Year: ");
		int year = scn.nextInt();
		System.out.print("Enter Month: ");
		int month = scn.nextInt();
		scn.close();

		if (year % 4 == 0 && year % 400 == 0 || year % 100 != 0) {
			System.out.println(year + " is a LeapYear");
		} else {
			System.out.println(year + " is not a LeapYear");
		}
		switch (month) {
		case 1:
			System.out.println("Jan 31-Days");
			break;
		case 2:
			if (year % 4 == 0 && year % 400 == 0 || year % 100 != 0) {
				System.out.println("Feb 29-Days");
			} else {
				System.out.println("Feb 28-Days");
			}
			break;
		case 3:
			System.out.println("March 31-Days");
			break;
		case 4:
			System.out.println("April 30-Days");
			break;
		case 5:
			System.out.println("May 31-Days");
			break;
		case 6:
			System.out.println("June 30-Days");
			break;
		case 7:
			System.out.println("July 31-Days");
			break;
		case 8:
			System.out.println("Aug 31-Days");
			break;
		case 9:
			System.out.println("Sep 30-Days");
			break;
		case 10:
			System.out.println("Oct 31-Days");
			break;
		case 11:
			System.out.println("Nov 30-Days");
			break;
		case 12:
			System.out.println("Dec 31-Days");
			break;
		default:
			System.out.println("Invalid Month");
		}
	}
}
