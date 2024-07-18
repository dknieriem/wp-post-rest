# WP Post REST

Exposes a REST endpoint at wp-json/wp-post-rest/v1 named 'getposts', with path parameter numPosts

Call it using a GET request at {your-site}/wp-json/wp-post-rest/v1/getposts/<code>integer</code> to return up to the <code>integer</code> most recent posts
Returns JSON array with 2 keys:

* 'posts' contains the post objects in an array.
* 'size' contains the size of the post array returned. This will vary from <code>integer</code> passed if there are fewer published posts than requested

# Discussion

This plugin is redundant, as the WP Rest API already has endpoints exposed for this:
[/wp-json/wp/v2/posts](https://developer.wordpress.org/rest-api/reference/posts/#definition)