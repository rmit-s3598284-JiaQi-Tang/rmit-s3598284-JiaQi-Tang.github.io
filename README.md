![Jacky](rmit-s3598284-JiaQi-Tang.github.io/images/IMG_5364.JPG)


You can click [here](https://github.com/rmit-s3598284-JiaQi-Tang/rmit-s3598284-JiaQi-Tang.github.io) to view the content of my github page!

My name is JiaQi Tang, born in 3rd/Dec/1993 ,studied at RMIT university from 2017

# **Samples of my works**

## [1.ELEVATOR SYSTEM](https://github.com/rmit-s3598284-JiaQi-Tang/Elevator)

![elevator uml](rmit-s3598284-JiaQi-Tang.github.io/images/ELEVATOR SYSTEM.png)

## [2.BINARY SEARCH](https://github.com/rmit-s3598284-JiaQi-Tang/BinarySearch)

```
import java.util.Scanner;

public class BinarySearchDemo {
	public int binarySearch(int[] nums, int target) {
		if (nums == null || nums.length == 0) {
			return -1;
		}
		int start = 0, end = nums.length - 1;
		while (start + 1 < end) {
			int mid = start + (end - start) / 2;
			if (nums[mid] < target) {
				start = mid + 1;
			} else if (nums[mid] > target) {
				end = mid;
			} else {
				end = mid;
			}
		}
		if (nums[start] == target) {
			return start;
		}
		if (nums[end] == target) {
			return end;
		}
		return -1;
	}

	public static void main(String[] args) {
		@SuppressWarnings("resource")
		Scanner userInput = new Scanner(System.in);
		int target;
		int size;
		System.out.println("Enter the size of the array");
		size = userInput.nextInt();
		int nums[] = new int[size];
		for (int numLoop = 0; numLoop < nums.length; numLoop++) {
			System.out.println("Please give a number:");
			if (numLoop == 0) {
				nums[numLoop] = userInput.nextInt();
			} else {
				boolean numberBigger = false;
				do {
					int nextInt = userInput.nextInt();
					if (nextInt > nums[numLoop - 1]) {
						nums[numLoop] = nextInt;
						numberBigger = true;
					} else {
						System.out.println("the new number has to be bigger than the last number");
					}
				} while (!numberBigger);
			}
		}
		System.out.println("please give the target");
		target = userInput.nextInt();
		BinarySearchDemo bs = new BinarySearchDemo();
		System.out.println("the array you have input is:" + java.util.Arrays.toString(nums));
		if (bs.binarySearch(nums, target) != -1) {
			System.out.println("the location of the target " + target + " is: " + bs.binarySearch(nums, target));
		} else {
			System.out.println("the target " + target + " is not found in the array");
		}
	}
}
```
## [3.Casino Dice Game in MVC](https://github.com/rmit-s3598284-JiaQi-Tang/CasinoDiceGame-SADI-assignment2-)

![diceGameFrameScreenShot](CasinoDiceGame-SADI-assignment2-/Screen Shot 2018-07-05 at 5.48.38 am.png)

## [4.TO BE CONTINUE..](https://github.com/rmit-s3598284-JiaQi-Tang)
