# Merge: this program takes two arrays and puts them together
import java.util.*;

public class Merge {
	public static void main(String[] args) {
		int[] a1 = {14, 44, 55, 66, 90};
		int[] a2 = {8, 69, 40, 33, 24};
		int[] a3 = merge(a1, a2);
		System.out.println(Arrays.toString(a3));
	}
	
	public static int[] merge(int[] a1, int[] a2) {
		int[] result = new int[a1.length + a2.length];
		for (int i = 0; i < a1.length; i++ ) {
			result[i] = a1[i];
		}
		for (int i = 0; i < a2.length; i++) {
			result[a1.length + i] = a2[i];
		}
		return result;
	}
}
