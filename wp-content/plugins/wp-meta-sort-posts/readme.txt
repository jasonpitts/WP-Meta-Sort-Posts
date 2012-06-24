WP-Meta-Sort-Posts
==================

This is a WordPress plugin that allows blog owners to create pages with lists of posts using custom queries specified in a shortcode.



WP Meta Sort Posts Plugin Shortcode Usage
=========================================
Create a new page and include a shortcode in the following format:
 
[msp query_string="QUERY"]
 
“QUERY” in the above example refers to a complete query in URL Query String format. Both Public and Private WordPress Query Variables can be passed as long as it is formatted appropriately. e.g.
 
[msp query_string="meta_key=shortcode_test&meta_value=Arizona&orderby=meta_value&order=asc"]
 
Notes: Do not URL Encode special characters like spaces to %20. Do not use query vars “paged” and “offset” in your shortcode because they are automatically calculated and added to the query string.
If you prefer, you can also pass each argument separately.
 
[msp Argument1=”Value1” Argument2=”Value2” Arguement3=”Value3”]
 
The same query will be performed as in the example above if the arguments are passed like this.
 
[msp meta_key="msp_test" meta_value="Arizona" orderby="meta_value" order="asc"]