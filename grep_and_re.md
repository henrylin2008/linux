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
	* **grep -n ABC grep.txt**: finding the line number of matching pattern 'ABC' on the file
		* -n: line number
		* ex: 32:ABC, 66:ABC
	* **grep -o AB grep.txt**: only shows matching pattern
		* ex: AB, AB, AB
		* ex: -o A.: AB, AC, AE, AD
	* **grep -C 4 A.A grep.txt**: show 4 lines before and after matching pattern A.A
		* -C k: shows k lines surrounding all matches 
		* ex: ATX, ATY, ATZ, AU, **AUA**, AXB, ACT, ADR, ADW

	* **ls | grep AB**: find all the files (in current directory) that has 'AB'
		* ex: ABC, BAB, EAB 
 	* **grep -r hello root**: find hello pattern from the files within root directory
 		* **-r**: recrusive
 		* ex: root/a.txt:hello, root/text2.txt:hello, root/abc.txt:hello

* **re**:
	* **.** 	  - Any Character Except New Line
	* **\d**      - Digit (0-9)
	* **\D**      - Not a Digit (0-9)
	* **\w**      - Word Character (a-z, A-Z, 0-9, _)
	* **\W**      - Not a Word Character
	* **\s**      - Whitespace (space, tab, newline)
	* **\S**      - Not Whitespace (space, tab, newline)

	* **\b**      - Word Boundary
	* **\B**      - Not a Word Boundary
	* **^**       - Beginning of a String
	* **$**       - End of a String

	* **[]**      - Matches Characters in brackets
	* **[^ ]**    - Matches Characters NOT in brackets
	* **|**       - Either Or
	* **( )**     - Group

	**Quantifiers:**
	* *	          - 0 or More
	* **+**       - 1 or More
	* **?**       - 0 or One
	* **{3}**     - Exact Number
	* **{3,4}**   - Range of Numbers (Minimum, Maximum)


	#### Sample Regexs ####

	[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+