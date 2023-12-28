<link rel="stylesheet" href="../css/notes.css" />

# TUTORIAL NOTES:

<a class="bookmark-link" href="#bookmark">JUMP TO BOOKMARK</a>

| **Tutorial Name**    | **Create a WordPress Plugin from Scratch [Playlist]**     |
| -------------------- | --------------------------------------------------------- |
| File Name            | NOTES.md                                                  |
| Date Created         | 12/28/23                                                  |
| Date Modified        | --                                                        |
| Platform             | Website                                                   |
| Channel              | [Elementor Developers](https://developers.elementor.com/) |
| Version              | 0.0.1                                                     |
| Programmer / Student | **Eric Hepperle**                                         |

* **Tutorial URL:** https://developers.elementor.com/docs/widgets/advanced-example/

---

## Dev Environment

### Install New Local WordPress Site

- Discourage search engine visibility

- **REPO FOLDER:** ehw-tutwrk-ele-oembed-widget
- **URL:** http://lardev-elsms.test/
- **Folder:** T:\Laragon\lardev-elsms\wp-content\plugins\ehw-tutwrk-ele-oembed-widget
- **WEB SERVER:** Laragon
- **GITHUB:** https://github.com/codewizard13/ehw-tutwrk-ele-oembed-widget


## Video 1

- Set `WP_DEBUG` to **true** in **wp-config.php**: This ensures that any errors will be displayed on screen.

#### #TIP: In the past we would have recommended to set WP_DEBUG back to false in production environments. However, this set of code leaves debugging enabled, logs it to a file, and doesn't display in views -- so no user sees the error messages unless they go and view the error.log file.

```php
// Enable WP_DEBUG mode
define( 'WP_DEBUG', true );

// Enable Debug logging to the /wp-content/debug.log file
define( 'WP_DEBUG_LOG', true );

// Disable display of errors and warnings
define( 'WP_DEBUG_DISPLAY', false );
@ini_set( 'display_errors', 0 ); // WPE auto-added this setting
```

---

- Navigate to `wp-content/plugins` folder
- Create new folder - the folder name will be same as your main PHP file

**#TIP:** To avoid any plugin name conflicts, in the WP Dashboard > Plugins > Click "Add New" and search for the plugin name that you want. This will tell you what plugins are likely to conflict so that you can give yours a unique enough name.


- Create plugin folder **alecaddd-plugin**
- Inside plugin folder create main plugin file **alecaddd-plugin.php**
- Add the following to main plugin file contents:

  - Declare package name: AlecadddPlugin

Create comment block as follows:

| Field        | Value                                                                               | Purpose                                                                        |
| ------------ | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| Plugin Name: | Alecaddd Plugin                                                                     |                                                                                |
| Plugin URI:  | http://alecaddd.com/plugin                                                          | The website that the plugin calls home                                         |
| Description: | This is my first attempt to write a custom Plugin for this amazing tutorial series. | Describe the plugin                                                            |
| Version:     | 1.0.0                                                                               | Version number                                                                 |
| Author:      | Alessandro "Alecadd" Castellani                                                     | Author name                                                                    |
| Author URI:  | http://alecaddd.com                                                                 | When the user clicks the author name, this is the website it will take them to |
| License:     | GPLv2 or later                                                                      | Use open source license                                                        |
| Text Domain: | alecadd-plugin                                                                      | Same as folder name                                                            |

**#GOTCHA:** Author says it is hard to release a plugin on official WP repository that is not open source so best just to use a GPL license.

## Create New WordPress Install for tutorial

Database Name: **tut_loc_alecadd_20230217**




--- --- ---

## Questions

  - **Q:** _Why is @package even necessary? What does it do?_


## Cleanup

- Set `WP_DEBUG` to false
- Enable search engine visibility



---


## BOOKMARK