// JAVA code to find
// duplicates in O(n) time

class Leet442 {

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

Output:- 

![image](https://user-images.githubusercontent.com/72159431/198515322-285c9a43-4592-44fa-9211-690cd90eccaf.png)
