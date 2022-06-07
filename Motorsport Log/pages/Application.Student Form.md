- [Student Form](https://docs.google.com/forms/d/e/1FAIpQLSfgbDc-6qODy7T19XOwc05JBa7KlDx7AbwS4II7ZX7PRszyZw/viewform)
  collapsed:: true
	- ![student_form.png](../assets/student_form_1653321610968_0.png)
- # Aptitude
	- This section is a bonus section, to see who will take the extra effort to fill this up
	- Correctness is **not** the major focus
	  id:: 6288a3ed-b2f0-4926-8db8-d68f3b1fb7fd
	- Involves [[Application/Point System]]
- # Implementation
  collapsed:: true
	- ## Input ID ~~year, discipline~~
	  collapsed:: true
		- ((d7c4bdfc-3566-41ef-85bb-eef131b597d8))
	- ## Derive year, discipline
	  collapsed:: true
		- ((4847faa0-cd7e-4f2f-bd35-7afab919f825))
		- Year
		  collapsed:: true
			- ```mysql
			  =ARRAYFORMULA(IF(ISBLANK(D2:D), "",
			  	IF( MONTH(TODAY()) > 6,
			  		YEAR(TODAY())-MID(D2:D, 1, 4)+1,
			  		YEAR(TODAY())-MID(D2:D, 1, 4)
			        )
			  ))
			  ```
		- Displine
		  collapsed:: true
			- ```mysql
			  =ARRAYFORMULA(IF(ISBLANK(D2:D), "",
			  	VLOOKUP(
			  		VLOOKUP(MID(D2:D, 5, 2),
			  		Disciplines!A:Z,
			  	2, FALSE)
			  ))
			  ```