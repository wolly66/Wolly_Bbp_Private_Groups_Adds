# Wolly_Bbp_Private_Groups_Adds


This class is written to add to the Private groups plugin   https://wordpress.org/plugins/bbp-private-groups/  a method to add a user to  group via code, plugins or themes a method to remove a user from a group, via code, plugins or themes.

Include this class in your plugin or theme, then, when you need to add or remove a user to a group,
instantiate the class:

 i.e.: $bbp_private_groups_adds = new Wolly_Bbp_Private_Groups_Adds( $user_id , $group );
 
 Please, if you do not pass $user_id AND $group, the class do nothing
 
 Then, if you want to add a user to a group call the add() method
 $bbp_private_groups_adds->add(); 
 
 if you want to remove a user from a group, call the remove method
 $bbp_private_groups_adds->remove(); 
 
 $user_id must be an integer
 
 $group must be:
 
		 * a string
     
		 * longer then 5 char
     
		 * first 5 chars must be: group
     
		 * others chars must be numeric. i.e. 1
     
