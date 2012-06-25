=== WP Meta Sort Posts ===
Contributors: jasonpitts
Donate link: http://jasonpitts.com/wp-meta-sort-posts-wordpress-plugin/
Tags: sort, posts, custom fields, meta, query vars, query_posts, meta_key, meta_value, arrange post order, change post order, custom post order, modify order, post order, sort posts, posts sort, order by, order by custom field, sort by custom field, reorder, alphabetical
Requires at least: 2.0.2
Tested up to: 3.4
Stable tag: 0.9
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This is a WordPress plugin that allows blog owners to create pages with lists of posts using custom queries specified in a shortcode.


== Description ==

I initially developed WP Meta Sort Posts plugin because I needed to be able to create archive-style pages for posts based on custom fields. I quickly realized that it would be just as easy to knock down all the walls and allow for custom sorted pages to be created based on any combination of WordPress query variables. WP Meta Sort Posts is still in its initial beta release and I welcome all feedback and feature suggestions.

== Installation ==


<strong>WP Meta Sort Posts Plugin Shortcode Usage</strong>
<br /><br />
Create a new page and include a shortcode in the following format:
<br /><br /> 
<code>[msp query_string="QUERY"]</code>
<br /><br /> 
“QUERY” in the above example refers to a complete query in URL Query String format. Both Public and Private WordPress Query Variables can be passed as long as it is formatted appropriately. e.g.
<br /><br /> 
<code>[msp query_string="meta_key=shortcode_test&meta_value=Arizona&orderby=meta_value&order=asc"]</code>
<br /><br /> 
Notes: Do not URL Encode special characters like spaces to %20. Do not use query vars “paged” and “offset” in your shortcode because they are automatically calculated and added to the query string.
If you prefer, you can also pass each argument separately.
<br /><br /> 
<code>[msp Argument1=”Value1” Argument2=”Value2” Argument3=”Value3”]</code>
<br /><br /> 
The same query will be performed as in the example above if the arguments are passed like this.
<br /><br /> 
<code>[msp meta_key="msp_test" meta_value="Arizona" orderby="meta_value" order="asc"]</code>
