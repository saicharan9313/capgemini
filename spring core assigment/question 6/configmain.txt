package Question6;

import org.springframework.context.ApplicationContext;
import org.springframework.context.annotation.AnnotationConfigApplicationContext;
import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;
import org.springframework.context.annotation.PropertySource;
import org.springframework.context.support.ClassPathXmlApplicationContext;

//import com.spring.basics.spring5steps.Spring5stepsPropertiesApplication;

@Configuration
@ComponentScan
@PropertySource("dbConfig.properties")
public class configmain {
	public static void main(String[] args) {
		ApplicationContext context = new ClassPathXmlApplicationContext("Q6.xml");
		config Config = (config) context.getBean("config");
		Config.display();
	}
	
}
