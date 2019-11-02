=== Clean Fresh Archives ===
Contributors: Viper007Bond, ELH
Tags: archive, archives, posts
Requires at least: 2.5
Tested up to: 3.3.1
Stable tag: trunk

Archive generator. Plugin cloned from clean-archives-reloaded.

== Description ==

Clean Archives Reloaded generates a list of all of your posts, sorted by month. It's enhanced with Javascript to allow collapsing and expanding of months.

It's highly efficient and won't kill your server with tons of MySQL queries.

= Demo =

Check out one of my sites' [archive page](https://emmanuelhmar.com/archives/).

== Installation ==

###Upgrading From A Previous Version###

To upgrade from a previous version of this plugin, delete the entire folder and files from the previous version of the plugin and then follow the installation instructions below.

###Installing The Plugin###

Extract all files from the ZIP file, making sure to keep the file structure intact, and then upload it to `/wp-content/plugins/`.

This should result in the following file structure:

`- wp-content
    - plugins
        - clean-archives-reloaded
            | readme.txt
            | clean-archives-reloaded.php`

Then just visit your admin area and activate the plugin.

**See Also:** ["Installing Plugins" article on the WP Codex](http://codex.wordpress.org/Managing_Plugins#Installing_Plugins)

###Using The Plugin###

Just create/edit a post or page and type `[cleanarchivesreloaded]` where you would like the archives list to show up. You can also use `[cartotalposts]` to show your total post count.

Example page contents:

`Here is all [cartotalposts] of my posts:

[cleanarchivesreloaded]`

Configure options via Settings -> Clean Archives.

== Frequently Asked Questions ==

= Does this plugin support other languages? =

Yes, it does. See the [WordPress Codex](http://codex.wordpress.org/Translating_WordPress) for details on how to make a translation file. Then just place the translation file, named `car-[value in wp-config].mo`, into the plugin's folder.

== Shortcode Tag Parameters ==

You can customize the list options on a per-call basis if you wish.

* `usejs` -- (`1` or `0`) use Javascript or not to collapse the months
* `monthorder` -- (`new` or `old`) show newest months or oldest months first
* `postorder` -- (`new` or `old`) show newest posts or oldest posts first within months

= Examples =

No Javascript:

`[cleanarchivesreloaded usejs="0"]`

Oldest months first, oldest posts first:

`[cleanarchivesreloaded monthorder="old" postorder="old"]`

== Original Plugin == 

https://wordpress.org/plugins/clean-archives-reloaded/

== ChangeLog ==

** 0.0.1 **
- fixed deprecated create_function
- changed plugin info and other texts from original plugin

** 0.0.2**
- changed version
- use esc_js instead of js_escape - deprecated

** 0.0.3 **
- Fix "Methods with the same name as their class will not be constructors in a future version of PHP"