# Mobile Friendly Navigation
A Mr CMS navigation app containing a widget to be used when you need multi-tier navigation as well as a mobile friendly navigation.

# Installation
Include the App files in to your solution through Visual Studio.

# Usage
In order to get the navigation app working first replace the navigation widget in your nav bar with "Mobile Friendly Navigation".

Next in your base layout add the following after the body tag:

	<div class="left-menu hidden-print"></div>
    <a class="menu-close close-left btn btn-primary" href='#'>Close</a>
    <div class="site-overlay hidden-print"></div>

After your navbar include the following:

	<!-- MobileNavArea -->
    <div class="mobile-action-nav hidden-print" id="sidebarmenu">
        <div id="sidebarmenu-bar">
            <div class="mobilemenu">
                <div class="pull-left">
                    <a id="left-menu-toggle" href="#" class="btn"><span class="glyphicon glyphicon-th-list"></span>&nbsp;&nbsp;Menu</a>
                </div>
                <div class="clearfix"></div>
            </div>
        </div>
    </div>
    <!-- /MobileNavArea -->

The first HTML block is what we use as a container for the left nav slide in on mobile. The second HTML block is the navbar which shows the button to action the mobile menu.

Make sure you are using @Styles.Render(AppStylesheetBundle.VirtualUrl) and @Scripts.Render(AppScriptBundle.VirtualUrl) in your _Layout for the scripts and CSS to be included. If you are managing this yourself, make sure to include the files from within Content\Scripts and Content\Styles.

# Screen Grabs

![Desktop View](https://mrcms.blob.core.windows.net/web/1/mobile-friendly-navigation/mobile-nav-1.png)
![Mobile Action Nav](https://mrcms.blob.core.windows.net/web/1/mobile-friendly-navigation/mobile-nav-2.png)
![Mobile View](https://mrcms.blob.core.windows.net/web/1/mobile-friendly-navigation/mobile-nav-3.png)

# Mr CMS Support
Version 0.5 +


# Known Issues
If after adding a page your new page does not show in the navigation, please clear the cache from System -> Clear Caches -> Clear.