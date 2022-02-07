1. DAY 1 LAB

	Running Open Timer on Linux Platform
	Command: ot-shell  


	![otshell](https://user-images.githubusercontent.com/98871313/152780573-5c0e4059-a758-40d3-a330-a5f7afc27978.PNG)


	SDC File:

	![sdc file](https://user-images.githubusercontent.com/98871313/152781068-a2dd3230-ffda-42aa-9e19-e2f0a6aac685.PNG)



	Verilog File:


	![verilog](https://user-images.githubusercontent.com/98871313/152781185-1a315869-cc48-491e-9643-2354ae65651d.PNG)


	Timing File:


	![timing file](https://user-images.githubusercontent.com/98871313/152781339-1c7fbf6e-1ddd-47c8-a61e-03c57959e613.PNG)


	Command: ot-shell -i run.tcl -o opentimer.log

	Output:

	![analysis](https://user-images.githubusercontent.com/98871313/152782091-95558929-65f2-4c2f-b345-2d91b9eee0e1.PNG)


	Timing Graph

	![timing graph](https://user-images.githubusercontent.com/98871313/152782144-20a3ac7d-dbef-4b53-bfa7-15f2cdae3037.PNG)
	


2. DAY 2 LAB

	Early Lib File
	
	![early lib file](https://user-images.githubusercontent.com/98871313/152783505-7b2039fb-f5d1-4099-9a6c-864d7cdf4682.PNG)
	
	
	Late Lib File
	
	![late lib file](https://user-images.githubusercontent.com/98871313/152783566-5b4860fe-b8ad-4638-9e33-fafe9d9d1673.PNG)
	
	
	SPEF Parsing
	
	![spef parsing](https://user-images.githubusercontent.com/98871313/152783650-49317c77-e9ec-4dbd-8a6a-a88438018d08.PNG)


	run.tcl file
	
	![run tcl](https://user-images.githubusercontent.com/98871313/152783716-a957f35b-38fa-4ea1-b2a7-5cb330c14436.PNG)
	
	
	Report Timing Output:
	
	![image](https://user-images.githubusercontent.com/98871313/152783880-c26302af-62b1-4cf8-ba7a-9200c889b500.png)
	
	
3. DAY 3 LAB 

	run.tcl
	
	
	![run tcl](https://user-images.githubusercontent.com/98871313/152784255-e28ebc36-a4e8-4ce6-8a43-53b810d8b9a4.PNG)
	
	
	out.txt 
	
	
	![out txt](https://user-images.githubusercontent.com/98871313/152784302-5c0ba40a-4ecd-4967-8e3e-d6ff971878c0.PNG)
	

4. DAY 4 LAB


5. DAY 5 LAB


	CPPR
	
	![cppr1](https://user-images.githubusercontent.com/98871313/152784700-0e4e75d2-0868-4334-a854-44ebe0d1d5da.PNG)


	ECO OUTPUT
	
		‌‌‌Startpoint    : F1:CK
	Endpoint      : F2:D
	Analysis type : max
	------------------------------------------------------
	       Type       Delay        Time   Dir  Description
	------------------------------------------------------
		pin     241.110     241.110  rise  F1:CK (DFFR_X2)
		pin     141.286     382.396  rise  F1:Q (DFFR_X2)
		pin       0.000     382.396  rise  U3:A (INV_X1)
		pin       7.920     390.316  fall  U3:ZN (INV_X1)
		pin       0.000     390.316  fall  U4:A (INV_X1)
		pin       6.926     397.242  rise  U4:ZN (INV_X1)
		pin       0.000     397.242  rise  U5:A1 (NAND2_X2)
		pin       5.697     402.940  fall  U5:ZN (NAND2_X2)
		pin       0.000     402.940  fall  U7:A2 (NOR2_X1)
		pin      21.266     424.206  rise  U7:ZN (NOR2_X1)
		pin       0.000     424.206  rise  F2:D (DFFR_X2)
	    arrival                 424.206        data arrival time

	related pin      94.645      94.645  rise  F2:CK (DFFR_X2)
	 constraint     -30.222      64.423        library setup_rising
	cppr credit       6.598      71.021
	   required                  71.021        data required time
	------------------------------------------------------
	      slack                -353.185        VIOLATED
	69.2
	62.6
	Startpoint    : F1:CK
	Endpoint      : F2:D
	Analysis type : max
	------------------------------------------------------
	       Type       Delay        Time   Dir  Description
	------------------------------------------------------
		pin     241.110     241.110  rise  F1:CK (DFFR_X2)
		pin     141.286     382.396  rise  F1:Q (DFFR_X2)
		pin       0.000     382.396  rise  U3:A (INV_X1)
		pin       7.920     390.316  fall  U3:ZN (INV_X1)
		pin       0.000     390.316  fall  U4:A (INV_X1)
		pin       6.926     397.242  rise  U4:ZN (INV_X1)
		pin       0.000     397.242  rise  U5:A1 (NAND2_X2)
		pin       5.697     402.940  fall  U5:ZN (NAND2_X2)
		pin       0.000     402.940  fall  U7:A2 (NOR2_X1)
		pin      21.266     424.206  rise  U7:ZN (NOR2_X1)
		pin       0.000     424.206  rise  F2:D (DFFR_X2)
	    arrival                 424.206        data arrival time

	related pin     130.395     130.395  rise  F2:CK (DFFR_X2)
	 constraint     -30.222     100.172        library setup_rising
	cppr credit       6.598     106.770
	   required                 106.770        data required time
	------------------------------------------------------
	      slack                -317.435        VIOLATED

	

	run,tcl file with ECO
	
	![run tcl file with eco changes](https://user-images.githubusercontent.com/98871313/152784881-b4d2c40f-4ce5-495f-8885-4afe291cd77a.PNG)




