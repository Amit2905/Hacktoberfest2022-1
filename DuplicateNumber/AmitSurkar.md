// JAVA code to find
// duplicates in O(n) time

class Duplicate {

	public static void main(String args[])
	{
		int numRay[] = { 0, 4, 3, 2, 7, 8, 2, 3, 1 };

		for (int i = 0; i < numRay.length; i++) {
			numRay[numRay[i] % numRay.length]
				= numRay[numRay[i] % numRay.length]
				+ numRay.length;
		}
		System.out.println("The repeating elements are : ");
		for (int i = 0; i < numRay.length; i++) {
			if (numRay[i] >= numRay.length * 2) {
				System.out.println(i + " ");
			}
		}
	}
}


Output :- 
![image](https://user-images.githubusercontent.com/72159431/198514115-c1e862ec-3b34-4daf-8935-6ebbe7ec48f5.png)
