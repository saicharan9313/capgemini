package junitbasics;

public class Assign1Q2 {

	int min=0,max=0;
	

	public Assign1Q2 array(int[] a)
	{
		
		Assign1Q2 k=new Assign1Q2();
		int[] b=new int[2];
		int max=0,min=a[0];
		for(int i=0;i<a.length;i++)
		{
			if(a[i]>max)
				max=a[i];
		}
		b[1]=max;
		for(int i=0;i<a.length;i++)
		{
			if(a[i]<min)
				min=a[i];
		}
		b[0]=min;
		
		k.max=max;
		k.min=min;
		return k;
		
		
	}

}