# Welcome!

This Java template lets you get started quickly with a simple one-page playground.

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }

String message = "Hello World!";
System.out.println(message);

//{ autofold
}

public void test() {
    		System.out.println("=================================");
		System.out.println("Using Sequential Stream");
		System.out.println("=================================");
		int[] array= {1,2,3,4,5,6,7,8,9,10};
		IntStream intArrStream=Arrays.stream(array);
		intArrStream.forEach(s->
		{
			System.out.println(s+" "+Thread.currentThread().getName());
		}
				);
 
		System.out.println("=================================");
		System.out.println("Using Parallel Stream");
		System.out.println("=================================");
		IntStream intParallelStream=Arrays.stream(array).parallel();
		intParallelStream.forEach(s->
		{
			System.out.println(s+" "+Thread.currentThread().getName());
		}
				);
}

}
//}
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced Java template](https://tech.io/select-repo/385)
