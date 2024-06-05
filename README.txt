INSTALLATION
============

1. Install and enable the J/K Navigation module as you normally would.
2. Download the jk navigation jQuery plugin from https://github.com/lbarchive/jquery-jknav
3. Unzip the jk navigation plugin into one of two possible folders:
   a. If you have the Libraries module enabled, unzip the plugin into the 
   sites/all/libraries/jknav folder, such that the resulting full path of
   the file is sites/all/libraries/jknav/jquery.jknav.min.js
   b. If you do not have the Libraries module installed, unzip the file
   into the module's js folder, so that the resulting file is either
   sites/all/modules/jk_navigation/js/jquery.jknav.min.js or
   sites/all/example.com/modules/jk_navigation/js/jquery.jknav.min.js
4. Give yourself and all administrators the "Administer J/K Navigation"
permission at admin/people/permissions#module-jk_navigation

CONFIGURATION
=============

1. login to your website as an administrator
2. visit the configuration page at Administer > Configuration >
User Interface > J/K Navigation or admin/config/user-interface/jk_navigation
3. The Navigation selector requires a little knowledge about how
the CSS selectors work. The default for the module assumes that 
comment headings are marked up with H3 tags and given the class
'comment-title', hence the default of 'h3.comment-title'. If you've
modified the way your comments are marked up, you will need to 
change this selector.
4. Other options:
  i. Select keys for Up and Down. The defaults are k for up and
  j for down.
  ii. (Optional) The Name option. You will probably not need to change
  this option.
  iii. Speed. "normal" should be good for most implementations.
  iv. Easing. From the jQuery documentation: "The only easing 
  implementations in the jQuery library are the default, called 
  swing, and one that progresses at a constant pace, called 
  linear." You will probably not need to change this option.
  v. At the end: 
    a. Circular: choosing this option will tell the module
    to come back to the top if you've reached the last element
    you cycle through.
    b. Stops at the end: choosing this option will tell the
    module to do nothing if you press j when reaching the
    last element
  vi. Start from:
    a. Last position: where you ended up last when you pressed
    the j or k key (or whatever you've set it to)
    b. Current position: where you are currently (this assumes
    you've scrolled up or down, and the module will attempt to
    calculate your position)
    
