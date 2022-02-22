package junitbasics;

import static org.junit.jupiter.api.Assertions.*;

import org.junit.jupiter.api.Test;

import static org.junit.jupiter.api.Assertions.*;
class InsufficientFundsExpcetionTest {

	@Test
	void test() {
		
		Assign1Q3 a=new Assign1Q3();
		assertThrows(InsufficientFundsExpcetion.class, ()->Assign1Q3.bank(50000));
		
		assertThrows(InsufficientFundsExpcetion.class, ()->Assign1Q3.bank(1000000));
	}

}