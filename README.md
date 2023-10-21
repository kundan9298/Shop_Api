			API			
	Base URL	http://127.0.0.1:8000/api/				
	Auth	Token Based				
	Token Provider	Login API				
	Token Package Name	Sanctum				
						
						
						
Profile	URL	Method	IS_Auth ?	Parameters	Retrun	
vendor	/register	POST	No	name, email, password, c_password		
	/login	POST	YES	email, password		
	/logout	POST	YES			
						
Product Add by vendor	/add	POST	YES	name, qty, color, size	Json, success, data, message, status	
	/delete/{id}	DELETE	YES	id		
	/update/{id}	POST	YES	id		
	/all_product	GET	YES			
						
						
User	/user_register	POST	No	name, email, password, c_password		
	/user_login	POST	YES	email, password		
	/user_logout	POST	Yes			
						
						
Product add to cart by User	/add_to_cart	POST	YES	qty, product_id, user_id	Json, success, data, message, status	
	/delete_from_cart/{id}	POST	YES	id		
	/cart_product_update/{id}	POST	YES	id		
	/view_all_cartData	GET	YES			
						
						
						
						
						
						
						
