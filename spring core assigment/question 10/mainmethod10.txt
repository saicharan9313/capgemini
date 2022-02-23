package Question10;

import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class mainmethod {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		ApplicationContext Context = new ClassPathXmlApplicationContext("Q10.xml");
		Details details = (Details) Context.getBean("detail");
		
		details.details();
	}

}
