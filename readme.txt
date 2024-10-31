=== Post Authorship ===
Contributors: JuanJedi
Tags: Post, Authorship, Author, Change Author Name
Version: 1.0
Requires at least: 3.5
Tested up to: 3.8
Stable tag: 1.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Allows to write manually the post's author display name.

== Description ==

In some cases you need to set a display name in a post without register a new user in your site.

So you have a large blog with a plenty users. And one day, you have to delete one of them, no matter why. You have to assign all its posts to other user. But the
original Author is that user you have just deleted! What can you do?

Here is a simple but effective solution. 

Post Authorship adds a new meta box to your posts. You can set a new Author name for the post, and, if your theme uses the "the_author" function to get the Author display name,
the plugin will write the name that you have set.

Also, the plugin will hide the link when your theme uses "the_author_posts_link". Obviously, you are writing a non-user name, so it doesn't have a posts archive page.

It allows .mo and .po translation files. The plugin supports:

* English, Spanish.

== Installation ==

1. Upload the directory to the `/wp-content/plugins/` directory.
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently asked questions ==

= Does the plugin set an Archive page for the new Author's name? =

No... Not yet. At the moment, this new name is just that, a display name. You write it and the plugin switch it when the_author or the_author_posts_link are used. 
In the next future I will investigate how can I do that. Stay tuned!

= Hey, this doesn't work... I wrote a new name, but my theme shows the original WordPress user name =

Oh, probably your theme is not compatible. Some themes don't use 'the_author' function to retrieve the post author. If this is your case, this plugin is not for you, because 
the plugin only knows how to modify 'the_author' and 'the_author_posts_link' functions. 

= My Theme uses 'the_author' function and the plugin doesn't work! =

Ok, in that case use the support forum and I will try to help you!

= Why the "About the author" box is showing the original WordPress user bio? =

The plugin only works with functions "the_author" and "the_author_posts_link". This means that other plugins or theme options which shows Author's Info boxes are not compatible 
with this plugin. They will get the WordPress Author info. You must disable this info box (individually for every post) when you change the Author's name using this plugin.

== Changelog ==
              
= 1.0 - 02/01/2014 =
* Basic functionality created: the plugin allows to change the Author's display name. 