xeno_ui_wip
===========

xeno_ui repo work in progress

## Widget

* Renameing a widget:
  * change class name
  * change class name in dev_app
  * change file name (*.coffee)
  * change directory name
  * change file path in main.coffee
  * change css name (*.css)
  * change css name in index.html
  * change css name in Gruntfile for production

* Templateing for widget
  * do NOT put comment on top of the file (when require it will also require comment)

## Test Channel Widget
* nothing will happen if no proper user yml is present, it is being request during open_channel()
  so must make sure that the file contains user list exists, and each user MUST present `account_id`:
  * `<seed_set>/config/ui_data.yml` in xeno_ui
  * `users/users.yml` in xenoui_recipe_generator
  * `students/ui_data.yml` in ofc-ui, NOTE there is NO `account_id` for this one
  * we should standardize this somehow!!
  * should NOT need account_id when `@settings["enable_signin"]` is false
  
## Action Menu Widget
 * in template generic option block for each taregt MUST defined and MUST placed at bottom position

## Tree Widget
* make sure in core.coffee there are a custom update_<xxx>_tree method for each tree instance
* make sure the icon is defined for all the node type 
  * because default icon will affect it's children, so when a node slected, the selected icon will affect it's children
  * but if the icon for each node type is defined properly, it won't happen. (see Example in jqtree.extend.icon.css)



