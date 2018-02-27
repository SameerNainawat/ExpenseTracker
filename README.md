<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
    pageEncoding="ISO-8859-1"%>
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=ISO-8859-1">
<title>Dashboard</title>

<link href="css/Dashboard.css" rel="stylesheet" type="text/css">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>	
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-select/1.12.4/css/bootstrap-select.min.css">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-select/1.12.4/js/bootstrap-select.min.js"></script>	
  <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script src="jquery-select7.js"></script>
  
	
<meta name="viewport" content="width=device-width, initial-scale=1">

<script>

$(".select7").select7()
</script>

</head>
<body>

<div class="container" style="max-width:100%;">
	
	<div class="row"> <!-- Row 1 --> 
	<div class="col-sm-3" style="background-color:lavender;">   <a href="Dashboard.jsp" id="logo"> <img src="img/small-logo.png" ><strong id="logoname">Sammy Studios</strong> </a>   	</div>
	<div class="col-sm-6" style="background-color:lavender;">		
			<ul>
				<li>	<a href="#">Overview </a>	</li>
				<li>	<a href="#">Transactions </a>	</li>
				<li>	<a href="#">Schedule </a>	</li>
				<li>	<a href="#">Goals </a>	</li>
				<li>	<a href="#">Reports </a>	</li>
			
			</ul>
	</div>			
	<div class="col-sm-3" style="background-color:lavender;">	
	
			<button type="button" class="btn btn-info btn-lg" data-toggle="modal" data-target="#myModal">+</button>
			
			  <!-- Modal -->
 			 <div class="modal fade" id="myModal" role="dialog">
  				  <div class="modal-dialog">
    
     					 	 <!-- Modal content-->
    				 <div class="modal-content">
    				       					  
       				      <button type="button" class="close" data-dismiss="modal">&times;</button>
         				 
      					  <div class="modal-body">
       				      
       				      	<form class="form js-form" action=""><!-- Form Modal for + button  -->
       				      	
       				      	<div class="btn-group control-group js-btn-group" data-toggle="buttons">
       				      		<label class="btn expense js-expense" id="fastadd-expense-btn" > <!-- Expense Button -->
       				      			<input type="radio" name="type" value="expense">
       				      			
       				      			    Expense
       				      			
       				      		</label>
       				      		
       				      		
       				      		<label class="btn income js-income" id="fastadd-income-btn" > <!-- Income Button -->
       				      			<input type="radio" name="type" value="income">
       				      			
       				      				Income
       				      			
       				      		</label>
       				      		
       				      		<label class="btn transfer js-transfer" id="fastadd-transfer-btn" > <!-- Transfer Button -->
       				      			<input type="radio" name="type" value="transfer">
       				      			
       				      				Transfer
       				      			
       				      		</label>
       				      		
       				      	</div>
       				      	
       				      	<div class="js-container">  <!-- Modal Form Feilds -->
       				      		<div>
       				      				<div class="form-row">
       				      					<input type="text" placeholder="Wallet" disabled style="width:100%;"/>
       				      				</div>		
       				      				
       				      				<div class="form-row">
       				      					<input type="text" class="amount calcinput-field field js-calcinput-field" name="amount" autocomplete="false" placeholder="0" />
       				      					<span class="currency">INR</span>
       				      				</div>
       				      				
       				      				<div class="form-row">
       				      					<select class="select7" style="width:100%;">
       				      						<option data-icon="img/pw_maze_black.png">	Miscellaneous   </option>
       				      						<option>	Bills			</option>
       				      						<option>	Business Expenses</option>
       				      						<option>	Dining Out		</option>
       				      						<option>	Education		</option>
       				      						<option>	Entertainment	</option>
      				      						<option>	Gift and Donations</option>
       				      						<option>	Groceries		</option>
       				      						<option>	Health and Fitness</option>
       				      						<option>	Home			</option>
       				      						<option>	Kids			</option>
       				      						<option>	Shopping		</option>
       				      						<option>	Tax and Fines	</option>
       				      						<option>	Transfer		</option>
       				      						<option>	Transport		</option>
       				      						<option>	Travel			</option>       				      						
       				      					</select>
       				      				</div>
       				      				
       				      				<div class="form-row">
       				      					<input type="date" name="date" id="date">
       				      				</div>
       				      				
       				      				<div class="form-row">
       				      					<input type="text" name="addnote" id="addnote" placeholder="Add notes, #tags and @payee">
       				      				</div>
       				      				
       				      				<div class="form-row">
       				      					
       				      					<input type="button" data-dismiss="modal" name="close" value="Close" class="bttn" />
       				      					<input type="submit" name="submit" value="Add" class="bttn"  />
       				      					
       				      				</div>
       				      				
       				      		</div>
       				       	</div>
       				      	
       				      	
       				      	
       				      	</form>
       				      
       					  </div>
       					  
       					  
     				 </div>
      
   				</div>
  			</div>
	</div>
	
	</div>	<!-- Row 1 ends here -->
	
	<div class="row">
		<div class="col-sm-3 sidenav ">
	
			<a href="#">Balance</a>
		
	
			<a href="#">Wallet</a>
		</div>
		
	</div>

</div>

<div class="row" id="footer" >
	
	<p>	Hand crafted by Sameer Nainawat.	</p>
	
</div>


</body>
</html>