 Instructions for the DecimalToRomanNumber_Refactoring exercise:

 	Please use ecipse and its automated refactorings and automated code completion proposal mechanisms for this exercise. Indeed, try to get eclipse to do as much of the code changes for you as possible, without either typing or copy/pasting. 
 
 	Please refactor this code until you can no longer make methods usefully smaller, 
 	and can no longer make classes themselves usefull smaller, meanwhile  keeping the existing end-to-end tests running green at all times. Run the tests as frequently as you can, and check in green-bar code frequently, in order to make it easy to revert to a green-bar state if you get in trouble with a particular refactoring. 

 	Follow the advice in Uncle Bob Martin's "Extract till You Drop" practice, as described in the blog post of the same name. 

 	As you introduce any new class, please retrofit a test for just its public API. 

 	Please note: while the existing tests run quickly in jUnit, they may or may not qualify as either "functional tests," "end-to-end tests," or "isolation tests," or "microtests." What do you think?
 	
 	The specific automated and manual refactorings you will use will likely be only these:
 	
 		--Rename
 		--Extract Method
 		--Extract Class/Enum (manual)
 		--Change Method Signature
 		--Pull Up method
 		--Change variable scope
 		--Move class
 


 	Are any of your classes or methods doing more work than they should, or holding more state than they should?

 	How can you tell?
 	
 	Another way to ask the same questions: are any of your classes and methods mixing together different domain ideas?

 	Indeed, what are the inherent domain ideas in this problem domain?
 	
 	Do a little google research to learn about the problem domain of converting decimal integers less than 4000 to Roman numbers. What terms do people use consistently and precisely? 
 	
 	What are the inherent operands (e.g., decimal number, decimal digit, decimal place)?  
 	What are the inherent operations and rules?
 	
 	What are the least confusing, most commonly used domain terms for these operands? 	
 	What terms do not have multiple definitions?
 	
 	("Roman Numeral," for example, seems to have at least two definitions.)

 	What domain ideas do you prefer for your implementation?
 	
 	--------------------------------------
 	Hint: From a useful definition of number "Place" on-line: 
 	http://www.factmonster.com/ipka/A0881929.html

		Decimal Places

		One decimal place to the left of the decimal point is the ones place. One decimal place to the right of the 
		decimal place is the tenths place.

		Keep your eye on the 9 in the visualization below to see where the decimal places fall.

		millions				9,000,000.0
		hundred thousands	  	900,000.0
		ten thousands	    	90,000.0
		thousands	      		9,000.0
		hundreds	         	900.0
		tens	           		90.0
		ones	             	9.0
		tenths	             	0.9
		hundredths	            0.09
		thousandths	            0.009
		ten thousandths	        0.0009
		hundred thousandths	    0.00009
		millionths	           	0.000009
 	-------------------------------------- 	
 	
 	List out your preferred terms for each domain idea (operand, operation, rule, etc) in a short glossary. 

 	How can you express each domain idea once and only once in the code? 
 	How can you name each package, class, and method consistently, using these domain terms?
 	
 	Given these terms, can you write short pseudo code to express what the algorithm is doing, and how it 

 	is doing it? Example:
 	
 	"Given a single decimal integer less than 4000 :
 		For each decimal place digit in the number, starting with ..."  


 	 --------------------------
 	 
 	Once you have finished the exercise once, delete your refactored code, and start over. 

 	Repeat the exercise from scratch for a total of 5 times. 

 	 --------------------------
   
 	Are you better off with a smallish class, with just a couple of smallish methods (one way to solve this problem), or with several tiny classes, each with tiny methods?  

 	While this domain provides a useful sandbox in which to practice "Extract till you Drop" (ala Uncle Bob Martin), how much extraction do you feel this problem domain truly deserves?	

 	Wny is it useful to know how to quickly "Extract till You Drop" in general? How might that be useful in real-life production programming?
 	
	
	
	
	
	
	