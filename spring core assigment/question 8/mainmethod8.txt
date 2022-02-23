package Question8;

import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class mainMethod {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("Q8.xml");
		sorting Sorting = (sorting) context.getBean("sort");
		
		int result = Sorting.sort(new int[] {1,2,3,4,5,6});
		System.out.println(result);
		
		context.close();
	}

}
