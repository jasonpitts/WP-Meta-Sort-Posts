WP-Meta-Sort-Posts
==================

This is a WordPress plugin that allows blog owners to create pages with lists of posts using custom queries specified in a shortcode.
<br /><br />

WP Meta Sort Posts Plugin Shortcode Usage
=========================================
Create a new page and include a shortcode in the following format:
 <br />
 <br />
[msp query_string="QUERY"]
 <br />
 <br />
“QUERY” in the above example refers to a complete query in URL Query String format. Both Public and Private WordPress Query Variables can be passed as long as it is formatted appropriately. e.g.
 <br /><br />
[msp query_string="meta_key=shortcode_test&meta_value=Arizona&orderby=meta_value&order=asc"]
 <br /><br />
Notes: Do not URL Encode special characters like spaces to %20. Do not use query vars “paged” and “offset” in your shortcode because they are automatically calculated and added to the query string.
If you prefer, you can also pass each argument separately.
 <br /><br />
[msp Argument1=”Value1” Argument2=”Value2” Arguement3=”Value3”]
 <br /><br />
The same query will be performed as in the example above if the arguments are passed like this.
 <br /><br />
[msp meta_key="msp_test" meta_value="Arizona" orderby="meta_value" order="asc"]
<br /><br />

To Do
==================
1.) Configurable Options for default loop<br />
2.) CSS options for default loop<br />
3.) Configurable  Nav Options<br />