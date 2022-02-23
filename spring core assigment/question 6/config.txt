package Question6;

import org.springframework.beans.factory.annotation.Value;
import org.springframework.context.annotation.PropertySource;
import org.springframework.stereotype.Component;

@Component
public class config {
	
	
	public String ClassName;
	
	
	public String Url;
	
	
	public String Username;
	
	
	public String Password;
	
	
	public String getClassName() {
		return ClassName;
	}
	public String getUrl() {
		return Url;
	}
	public String getUsername() {
		return Username;
	}
	public String getPassword() {
		return Password;
	}
	
	@Value("${driver_class}")
	public void setClassName(String className) {
		ClassName = className;
	}
	
	@Value("${external.service.url}")
	public void setUrl(String url) {
		Url = url;
	}
	
	@Value("${username}")
	public void setUsername(String username) {
		Username = username;
	}
	
	@Value("${password}")
	public void setPassword(String password) {
		Password = password;
	}
	public void display(){
		System.out.println("Driver : "+getClassName());
		System.out.println("URL : "+getUrl());
		System.out.println("User Name : "+getUsername());
		System.out.println("Password : "+getPassword());
	}
}
