=== Image Projector - a lightbox ===
Plugin Name: Image Projector
Contributors: wpgloe
Tags: lightbox, image, viewer, photo, slide
Requires at least: 5.3
Tested up to: 6.6
Stable tag: 5.11
Requires PHP: 7.4
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A unique, quiet, plug-and-play lightbox and image slider that let the visitor change viewing format, background and more.


== Description ==
Image Projector - a unique lightbox that provides a responsive full-window view and slider for images in posts or pages, including galleries and carousels. Developed for photos, useful for all types of images.


**Features**

 * Plug and Play, no editing of code needed 
 * Context-dependent image collections automatically created 
 * Tolerant to markup variations
 * Suitable for both block themes and classic themes
 * Modify strings - translate front end to targeted language region, RTL support.
 * Visitor can switch view style and background 
 * Zoom, pan 
 * Autoplay  
 * Optional thumbstrip when relevant 
 * Optional support for flipping image and viewing image in grayscale 
 * Smooth navigation with mouse, wheel, keyboard or touch gestures  
 * Static controls that does not jump with the image size
 * Uses on-demand image loading and preloading - fast startup  
 * Supports modern image formats WebP and AVIF when browser supports it
 * Humble and quiet appearance
 
**Demo**

Collection based on first or featured image in posts. Used on an **[archive page](http://www.lystfotograf.net/tags/fog "A tag archive page on lystfotograf.net")**, it will limit the collection to the images in queried posts (typically category and tag results or search results). 

Check out examples of standard behaviour - it may also well be used in combination with 3rd party or WordPress native **[galleries](http://www.image-projector.com/examples "image-projector.com/examples")**.

For available admin options, please see **[settings](http://www.image-projector.com/settings "image-projector.com/settings")**.

**Privacy Notice**

This plugin does not track users. It does not store any data to the database other than plugin settings, neither does it send any data to any server.

Last used view style and background style is stored in a cookie on visitor's device and applied if visitor returns.


== Installation ==
**New installation:**
1. Upload the plugin to your WordPress plugin directory or install it by using the "Add Plugin" function of WordPress
2. Activate the plugin at the plugin administration page.
3. Modify the plugin settings as needed and save changes.
 
**Update existing installation:**

Press the Update button for the plugin or follow these steps:

1. Download zip file from WordPress plugin directory.
2. Deactivate the plugin.
3. Unzip the downloaded file to the plugin folder.
4. Activate the plugin. If any new options are added, check the settings pages and adjust settings as needed.


== Frequently Asked Questions ==
-or possibly frequently asked...

= Why did you make this plugin when there are so many others to chose from? =
Good question! Being a photo enthusiast having a WordPress site with one post per image, I realized after a while that there were limited possibilities to show the images in a smooth flow.

To avoid the cumbersome manual navigation between posts, I decided to (try to) write a plugin to collect the featured image (if it has a featured image) or first image from each post, show them in an image slider and then navigate to the post from the image. The content of the slider is then defined based on the context of the page, for intance an archive page that contain the result of a tag query. 

Messing around with various gallery plugins - that always require som extra effort to set up - or modifying page template code was not an option.

Eventually the plugin was extended to be applied for general use as well, and the collection of post images and handling of navigation between posts has just become an optional feature that can be turned on/off from the plugin settings page.

= Are there any shortcut keys available? =

Yes, for those users who are blessed with a keyboard:  

**right arrow/left arrow** - next/previous  
**C** - toggle caption if supported  
**A** or **P** - toggle autoplay  
**B** - switch background class  
**L** - last image  
**T** - swith between slide in/out or cross-fade transition  
**V** or **S** - switch view style  
**X** - exit  
**Z** - zoom mode on/off  

= Which touch gesture or mouse operations are supported? =
**swipe left/right** go to next/previous image
**spipe up/down** exit viewer
**pinch** - zoom   
**doubleclick/doubletap** - enter/exit zoom mode  
**left mouse button down while swiping right/left with mouse** - next/previous  
**ctrl key and left mouse button down while swiping up/down** - enter zoom mode and do zooming  
**mousewheel** - zoom when in zoom mode  
**click caption** - turn off display of caption if captions are supported. Turn it on again from menu.  

= Only one image from a gallery or carousel is shown, and no arrows - why? = 
Probably due to that the the gallery or carousel wrapper is not detected. Please specify the parent element to all the gallery or carousel elements. If in doubt, do not hesitate to file a support ticket.

= Can I choose which posts/pages and images it shall be activated for? =
Yes. This can be specified in the plugin settings page.

= Can I modify the styles? =
Yes. Please have a look into the plugin settings page and the stylesheet located in the plugin directory. If you need advice on how to set up the styles, please leave a support message.

= Is it responsive and touch-device friendly? =
Yes, I would say so. 

= Does it work in all versions of all browsers? =
Visitors running a 'modern' browser released in 2020 or after should be good to go.

= How can I use it together with NextGEN gallery or other third-party galleries?
For NextGEN, select None for Lightbox effects in the Other options page of NextGEN gallery plugin.
For other galleries, please leave a support message if you are not able to make it work as expected.

== Screenshots ==

1. Full window with cut-off activated.
2. Image with frame.
3. Image with frame, showing thumbstrip.
4. Inside square on dark background. Right-click or click menu icon to show menu.
5. Typical settings page.

== Changelog ==
= 5.11 =
* Added option in Images to specify search depth in DOM tree for improved control of image collection.
* Correction to avoid use of an undefined variable that could case js error in some situations.
* Minor updates.
= 5.10 =
* Added options in Timings to modify message to visitor if slow connection or if an image failed to load.
* Added support for RTL language in front end menu and tooltip.
* Extended options in Controls for further flexibility.
* Minor updates.
= 5.9 =
* Added option in Features to control caption content.
* Improved image selection in picture tags.
* Minor updates.
* Tested for WordPress 6.6.
= 5.8 =
* Enhanced string translation in Translations to control both menu string and tooltip string.
* Adjustments to the button visibility settings in Control page.
* Tested for WordPress 6.5.
= 5.7 =
* Added settings section Translations for translating or otherwise modifying strings that appear in the front-end menu and tooltips.
= 5.6.2 =
* Fixed image size issue on Firefox causing width and height not to correspond to actual image.
= 5.6.1 =
* Fixed icon display issue revealed on Firefox browser.
= 5.6 =
* Glitch introduced in 5.5 related to swipe velocity fixed.
= 5.5 =
* Added option in Features to control if Download command shall be available.
Availability can be limited to logged-in users. In case it is activated, Download command will be added to the menu. It will only be available for images located at the same domain as the page being viewed.
* Added option in Controls to hide 'X' and zoom button on touch devices to simplify interface. Close and zoom can be controlled by commonly known touch gestures like swipe up/down or tap background to close, pinch in or double-tap to activate zooming.
* Minor general improvements.
* Tested for WordPress 6.4.
= 5.4 =
* Zoom - click on displayed zoom factor to show image in 1:1.
* Image counter - added more options to control display of the counter.
* Fixed error setting zoom center when pinching in view style 1.
= 5.3 =
* Late css loading revealed issues on certain themes. Moved css loading back to header.
* Added option in Features to show image counter. Default off.
* Now showing current image scale together with current zoom factor when zoom is active.
= 5.2 =
* Improvements to the full image and thumb image collection process.
= 5.1 =
* Removed use of file_get_contents that was used to load icon definition into page. Some servers may not be set up to allow this, resulting in no icons shown. Icon href now links to icon in svg sprite file included in the plugin.
* Fixed glitch that could cause a low resolution version of the image to be selected for viewing.