package junitbasics;

import static org.junit.jupiter.api.Assertions.*;

import org.junit.jupiter.api.Test;

class AssingmentQ2Test {

	@Test
	void test() {
		Assign1Q2 a=new Assign1Q2();
		int[] k= {45,78,2,65,87,13,6};
		assertEquals(2,a.array(k).min);
		assertEquals(87,a.array(k).max);
		
		int[] m= {1,2,3,4,5,6,7,8,9,10};
		assertEquals(1,a.array(m).min);
		assertEquals(10,a.array(m).max);
		
		int[] l= {10,20,30,40,50,60,70,80,90};
		assertEquals(10,a.array(l).min);
		assertEquals(90,a.array(l).max);
	}

}