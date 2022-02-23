package Question1;

import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		ApplicationContext context = new ClassPathXmlApplicationContext("Q1.xml");
		
		/*
		 * Customer customer = (Customer) context.getBean("Customer1");
		 * customer.details();
		 */
		
		
		  Customer customer1 = (Customer) context.getBean("Customer2");
		  customer1.details();
		 
	}

}
