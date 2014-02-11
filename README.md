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
  so must make sure that the file contains user list exists:
  * `<seed_set>/config/ui_data.yml` in xeno_ui
  * `users/users.yml' in xenoui_recipe_generator
  * we should standardize this somehow later
  
## Action Menu Widget
 * in template generic option block for each taregt MUST defined and MUST placed at bottom position
