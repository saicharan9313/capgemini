package Question8;

import java.util.Arrays;

import javax.annotation.PostConstruct;
import javax.annotation.PreDestroy;

import org.springframework.beans.factory.DisposableBean;
import org.springframework.beans.factory.InitializingBean;

public class sorting {
	
	public int sort(int [] numlist) {
		Arrays.sort(numlist);
		return numlist[numlist.length-1];
	}

	public void afterPropertiesSet() {
		// TODO Auto-generated method stub
		System.out.println("Bean Has Initialized");
	}

	public void destroy() {
		// TODO Auto-generated method stub
		System.out.println("Bean Has Desposed");
	}
	
	@PostConstruct
	public void pConstruct(){
		System.out.println("postcontruction of bean");
	}
	
	@PreDestroy
	public void pdestroy(){
		System.out.println("predestroy of bean");
	}
}
