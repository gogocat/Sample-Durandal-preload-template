Sample-Durandal-preload-template
================================

An example of Durandal js with preload template ability.

I have been using Durandal JS for a while and I think it is a fantastic framework.

However it lacks of option to preloading templates for fast view render. Probably because Durandal is using RequireJs text plugin for template loading.

So I modified the text.js

Yes, the change require jQuery.

The change was surprisingly simple and without breaking Durandal's binding life cycle.

An example of preloading the shell template on the index.html

	<script type="text/html" data-view-path="app/views/shell.html"> 
	... template content...
	</script>

Download this example and run in your local web server.

Open network inspector to see the difference.

Original source is from [Durandal Starter Kit](http://durandaljs.com/get-started.html) 