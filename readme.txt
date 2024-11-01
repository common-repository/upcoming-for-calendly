=== Upcoming for Calendly ===
Contributors: justdave
Tags: calendly, calendly-api
Requires at least: 5.8
Tested up to: 6.2
Stable tag: 1.2.3
Requires PHP: 7.2
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Display a list of upcoming already-scheduled Calendly events that still have open slots, and link to their specific registration pages.

== Description ==

# Upcoming Events Registration List for Calendly

This WordPress plugin adds a shortcode to list upcoming scheduled events from Calendly using the Calendly API and offers registration links for already-scheduled group events that still have open slots. You can either list all of your scheduled events, or restrict it to a specific event type.

To set it up, you will need to log into Calendly and generate an Access Token.  A link to do so is provided on the settings page. Paste the token into the box on the settings page.

To use it, place the shortcode `[upcoming-for-calendly]` on a post or page where you want the list to appear. To restrict it to a specific event type, use `[upcoming-for-calendly event="Event Type Name"]`.

The plugin currently implements a feature I needed. I am open to adding additional features that can be implemented via Calendly's API if there is a need for them.

Bug reports and feature requests can be filed at the [GitHub repository](https://github.com/justdave/upcoming-for-calendly/issues).

== Screenshots ==
1. List of upcoming events
2. List with no events available

== Changelog ==
#### 1.2.3 / 2023-04-18

* Make the description easier to read on wordpress.org

#### 1.2.2 / 2023-04-18

* Corrections to WP.org deployment process

#### 1.2.1 / 2023-04-18

* Autodeploy to WordPress Plugin Directory on new release

#### 1.2 / 2023-04-15

* Use WP HTTP API instead of the PHP Curl library
* Sanitize and escape, and use WP functions for it instead of built-in PHP functions
* Don't use underscore prefixes on functions that aren't in a class

#### 1.1.1 / 2023-01-12

* structured plugin zip file for wordpress.org plugin directory

#### 1.1 / 2023-01-09

* add a 'Settings' link on the Plugins page
* validate the Access Token before saving it on settings page
* don't hit the Calendly API on the settings page if there isn't an Access Token yet
* filter events before counting them, so "no events scheduled" message will still appear when other event types have events

#### 1.0.1 / 2023-01-07

* Display a message in shortcode output if there are no events to show

#### 1.0 / 2023-01-07

* Initial release.
