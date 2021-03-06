ACF QuickEdit Fields
====================

WordPress plugin which extends the functionality of the Advanced Custom Fields Plugin (Pro, Version 5+).  
http://www.advancedcustomfields.com/pro/

Show Advanced Custom Fields in list tables. Some columns are sortable.  
Edit field values in Quick Edit and / or Bulk edit.

Proofed to work with ACF Pro 5.x.  
Will not work with ACF Free (version 4.x).  
Requires at least PHP 5.3.
Tested with WordPress up to 4.9

See the [wiki](https://github.com/mcguffin/acf-quick-edit-fields/wiki) for a quick start and a list of [supported ACF Fields](https://github.com/mcguffin/acf-quick-edit-fields/wiki/Supported-ACF-Fields).

A note on sortable Columns: Sorting works over a meta query. As a result, items with an
unset ACF-Value will disappear from the list. To adjust or suppress sortability for a specific field use
`acf_quick_edit_sortable_column_{$field_name}` filter.


Getting started
---------------

 - Download the [latest release](../../releases/latest) zip file.
 - Rename the file to `acf-quick-edit-fields.zip` and install it like a regular WordPress plugin.
 - As long as the plugin is active it will check for Updates here on GitHub.


Developing
----------

This plugin uses gulp.

To get started `cd` in the plugin directory,  
run `npm install`  
followed by `gulp`.


ToDo:
-----

 - [x] QE+BE: Checkboxes with Custom -> Add Choice
 - [x] JS bindValidation
 - [x] BE: new fields js
 - [x] JS inlineEditTax
 - [x] Bug: validation: do not validate do-not-change
 - [x] Add plugin version number to enqueue script
 - [x] Allow QuickEdit for grouped fields
 - [?] Bug: QE -> save -> reload|navigate: Browser warning about unsaved changes.
 - [ ] Bug: Password field always saves empty value
 - [ ] Radio/Checkbox with Other: load other value(s) not shown after save (need to reload)
 - [ ] Support Taxonomy QE / BE
