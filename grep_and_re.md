* **grep pattern file**
	* **grep A. grep.txt**: any pattern starts with A and follow by any character
		* ex: Ab, ac, ad, NAB, PAO, PAQ 
	* **grep A.A grep.txt**: any pattern starts with A and ends with A
		* ex: ABA, ACA, AWA, ALA 
	* **grep [A,B].A grep.txt**: any pattern stars with A or B, follow by any character/s, and end with A 
		* ex: ABA, AHA, AOA, AUA, BBA, BCA, BIA, BZA 
	* **grep "A.B\|B.A" grep.txt**: '\|'= **or**, any pattern either starts with A followed by any character and ending with B, or starts with B followed by any character and ending with A
		* ex: ABB, ACB, BAA, BCA, BEA
	* **grep AB$ grep.txt**: match any pattern ending with 'AB'
		* ex: AAB, BAB, KAB, TAB, AB
	* **grep ^AB grep.txt**: match any pattern starts with 'AB'
		* ex: ABA, ABB, ABF, ABG
	* **grep -n ABC grep.txt**: finding the line number of matching pattern 'ABC'