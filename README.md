#jQuery Plugin Skeleton
##What?
Simple, it's just a skeleton of a jQuery plugin that you can download, clone, fork, whatever. I'm putting it on Github mainly for myself. It also includes an MIT license at the top of the skeleton.

##How?
Only thing you really have to do is edit the MIT license on the first line:

    Copyright (c) <Year> <First & Last Name>, <Your Web Site>

And then name your plugin by replacing "`pluginname`" here:

    pluginname: function(options) {
    
And once more replace "`pluginname`" here:

    $.error('Method ' + method + ' does not exist on jQuery.PluginName');

Finally you can add more code the `init` method, or add methods of your own in the `method` variable
found on line 16:

    var methods = {
    	init: function(options) {
			console.log(options);
			return this.each(function() {
				if(options) $.extend(settings, options);
				var $this = $(this);
				
			});
		}
	};

##Note!
This plugin allows you to keep on chaining, so, for example:

    $('#myelement').pluginname().css({border:'1px solid blue'});

Would run `pluginname` name on `#myelement` then add a blue border to it after.

##Whats next?

A skeleton that includes ready-to-go functions and callbacks for AJAX based plugins.

##Found a bug? 

Submit a bug report above or here: 

<https://github.com/OscarGodson/jQuery-Plugin-Skeleton/issues>