#jQuery Plugin Skeleton
##What?
Simple, it's just a skeleton of a jQuery plugin that you can download, clone, fork, whatever. 
This skeleton follows best practice and provides a quick framework for rapid plugin development.

##How?
First change first line of the MIT license to have your information:

    Copyright (c) <Year> <First & Last Name>, <Your Web Site>

And then name your plugin by replacing "`PluginName`" on line 37:

    PluginName: function(method) {
    
And once more replace "`PluginName`" on line 43:

    $.error('Method ' + method + ' does not exist on jQuery.PluginName');

Finally you can add more code the `init` method, or add methods of your own in the `method` variable
found on line 26:

	var methods = {
		init: function(options) {
			return this.each(function() { //ensures chainability
				if(options) $.extend(settings, options);
				var $this = $(this);
				//YOUR INIT CODE HERE
			});
		}
	};

##Note!
This plugin allows you to keep on chaining, so, for example:

    $('#myelement').PluginName().css({border:'1px solid blue'});

Would run the `init` function on elements matching `#myelement` then add a blue border to it after.

##Whats next?

A skeleton that includes ready-to-go functions and callbacks for AJAX based plugins.

##Found a bug? 

Submit a bug report above or here: 

<https://github.com/OscarGodson/jQuery-Plugin-Skeleton/issues>