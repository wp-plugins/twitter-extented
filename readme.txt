=== Twitter for Wordpress Extended 2 ===

Contributors: moroandrea

Tags: twitter, widget

Requires at least: 2.1

Tested up to: 3.1

Stable tag: 1.0.3.1


Twitter for WordPress Extended 2 shows your tweets, tweets for a search term (e.g. a tag), your friends timeline or the current twitter trends.


== Description ==

Twitter for WordPress displays yours tweets, your friends timeline, a Twitter search result or the current twitter trends in your WordPress blog. This is done by using the built in widget or by using PHP functions in your theme.


= Features =

	* Simply
	* Customizable
	* Widget support
	* No options page (yes, this is a feature if you consider that other plug-in cannot be inserted in your site more than once due to this)
	* Uses Wordpress resources (no extra files needed)
	* Detects URLs, e-mail address and @username replies


= Usage =

If you use WordPress widgets, just drag the widget into your sidebar and configure. If widgets are not your things, use the following php code to display Twitter messages:

`<?php twitter_messages("username"); ?>`

A number of options are available like:

	* specifying the number of the elements that should appear in your list via the $num parameter;
	* let the elements appear into an HTML list via the $list parameter
	* show the time when the tweet has been published via the $update parameter
	* transform text into an active link via the $hyperlinks parameter and apply a nofollow decoration with the $nofollowattribute
	* exclude retweets via the $excludeRT parameter
	* or don't include tweets that contain a particular text via $excludeText parameter (you can pass a simple string, or an array of values comma separated) 

If you want to display tweets to a special search result, use the following code:

`<?php twitter_searchstring("#twitaly"); ?>`


If you want to display the tweets of your friends timeline, use this:
`<?php twitter_friends( "username", "password" ); ?>`

If you want to display the current twitter trends, use that snippet:
`<?php twitter_trends(); ?>`

= Customization =

The plug in provides the following CSS classes:
	* ul.twitter: the main ul (if list is activated)
	* li.twitter-item: the ul items (if list is activated)
	* p.twitter-message: each one of the paragraphs (if msgs > 1)
	* .twitter-timestamp: the timestamp span class
	* a.twitter-link: the tweet link class
	* a.twitter-user: the @username reply link class
	* li.twitter-item img: format the avatar icon on search results

== Installation ==

Drop "twitter-for-wordpress-extended" folder (or even twitter_extended.php) into /wp-content/plugins/ and activate the plug in the Wordpress admin area.

If you use the "Twitter for Wordpress" plugin please deactivate it before activating "Twitter for WordPress Extended". The extended plugin is designed to replace the original.


== Credits ==
[Ricardo González](http://rick.jinlabs.com/) - The plugin is highly based on the plugin "Twitter for Wordpress", so the major part of the credits goes to him.
[Marc Schieferdecker](http://www.das-motorrad-blog.de/meine-wordpress-plugins/), The plugin fork from which this extension is derived.

== Contact ==

Any Suggestions? 
As I'm not a PHP programmer and I'm not going to support this fork actively, I will be glad to hear from you. Maybe that if the request or the suggestion is interesting enough I can spend some time on the development.


