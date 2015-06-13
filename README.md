# Id-to-variables
Direct access to elements through their id 

The function _id2public_var() dynamically converts elements ids in members of object E. 


Code : 

function _id2public_var(){ 
				var all = document.getElementsByTagName("*"); 
				 ={}          
				for (var i=0, max=all.length; i<max; i++){ 
					if(all[i].id!='') E[all[i].id]=all[i] 
				}          
			}          
	_id2public_var() 
	alert(E.two.style.color) 

	Special care should be taken as IDs need to be unique and later added elements would require recalling the function in order to have references ready to use in the window.E object
