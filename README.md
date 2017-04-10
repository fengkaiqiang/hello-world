# hello-world
just another repository
class Demo    //创建类
{
	//选择排序法
	public static void selectsort(int[] arr)
	{
		for (int x=0;x<arr.length-1 ;x++ )
		{
			for (int y=x+1;y<arr.length ;y++ )
			{
				if (arr[x]>arr[y])
				{
					int temp = arr[x];
					arr[x] = arr[y];
					arr[y] = temp;
					
				}
			}
		}
		
	}

	//冒泡排序法

	public static void bubblesort(int[] arr)
	{
		for (int x=0;x<arr.length-1 ;x++ )
		{
			for (int y=0;y<arr.length-x-1 ;y++ )
			{
				if (arr[y]>arr[y+1])
				{
					int temp = arr[y];
					arr[y] = arr[y+1];
					arr[y+1] = temp;
					
				}
			}
		}
		
	}


	//打印函数
	public static void printarr(int[] arr)
	{
		System.out.print("[");

		for (int x=0;x<arr.length ;x++ )
		 {
			 if (x!=arr.length-1)		
			System.out.print(arr[x]+", ");
			else
			System.out.println(arr[x]+"]");
		 }
	
	}


	public static void main(String[] args)
	{
		int[] arr = {1,2,85,84,566};
		printarr(arr);
		bubblesort(arr);
		printarr(arr);

	
	}

}

