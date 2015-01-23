#Loose list of ideas for fixes

I should write more issues. Most of the things I keep ranting about never make it to the issue tracker. Shame on me.

##Spicing up the uber searchbar

Searching for resources/elements in the uberbar is very limited. I would like to see search by fieldname for resources and by id for elements.

The github PR below already contains a few improvements:

###Use fieldname::value syntax to search for specific things

* id::32 - Any element/resource with id 32
* class_key::mgResource - Any moreGallery resource
* deleted::1 - Deleted resources
* introtext:LIKE::%foo% - Any resource containing the string %foo%

###New system setting uberbar_maxresults

Change default value of 5 results per category to another value.

###JSON search
An optional search by a complex json string would be even more awesome.

###Github:

* https://github.com/modxcms/revolution/issues/12283
* https://github.com/modxcms/revolution/pull/12282

##Get rid of style inconsistancies for tvs moved by form customization

If you move tvs to modx-resource-main-left/right there are a whole lot of things going wrong...

###Github:

* https://github.com/modxcms/revolution/issues/12221

##Changing xtype settings for some system settings to numberfield

xtype numberfield is only used for 'root_tree_id' all other system settings that require a number (site_start, etc) are set to textfield

###Github:

* https://github.com/modxcms/revolution/issues/12284

##Add numberfield to list of available xtypes for new system settings

Create a new system setting and try to picke numberfield from the list of available xtypes.

Its not in the list.

##Move messages away from system settings into lexicon files

A couple of system messages are still stuck inside system settings. 

```
site_unavailable_message
emailsubject
forgot_login_email
signupemail_message
webpwdreminder_message
websignupemail_message
````

Let's do something about it.

###Github:
https://github.com/modxcms/revolution/issues/6092

###Github:
https://mac.github.com/

###Github:

* To be announced...

#Loose list of ideas for plugins/extensions

##Make managerBreadCrumbs a standalone plugin

modDevTools by argnist shows breadcrumbs below each resource pagetitle.
They are quite useful and I think they should be a standalone extension.

###My plugin code on Github:

* https://gist.github.com/pepebe/f77f90ddfae1fcdca9a1


