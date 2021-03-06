mercury_fulltext
==============
A fork of the original [mercury_fulltext](https://github.com/HenryQW/mercury_fulltext) that supports using a self-hosted [Mercury Parser API](https://github.com/postlight/mercury-parser-api). Rest of original README continues below:

A Tiny Tiny RSS plugin written for [tt-rss](https://tt-rss.org) as a replacement for the grandpa-old plugin [af_readability](https://git.tt-rss.org/fox/tt-rss/src/master/plugins/af_readability), which doesn't work well for many RSS sites I subscribe to.

It utilizes [Mercury Parser](https://mercury.postlight.com/web-parser/) to extract the full content for feeds. ~~An API key is required to use this plugin, which is available for free [here](https://mercury.postlight.com/web-parser/)~~. 

It's made open source on GitHub [postlight/mercury-parser](https://github.com/postlight/mercury-parser).

## Warning

**Mercury API will be shutting down** in the future, please read more [here](https://postlight.com/trackchanges/mercury-goes-open-source)

You'are advised to host your own mercury instance, thus **this repo will be deprecated** in the future. For a dockerized self-host solution, please visit my repo [mercury-parser-api](https://github.com/HenryQW/mercury-parser-api).

Tested on BBC, The New York Times, The Verge, Cult of Mac, iDownloadBlog etc, in which af_readability can't handle the content properly.

**Some feeds may not render properly, if Mercury can't handle it.** Eg. BBC video-only feeds.

Installation
------------------------

Clone the repo into your tt-rss **plugins** folder.

Configuration
------------------------
The configuration is identical to af_readability, except you have to save your API key.

1. Enable the plugin *mercury_fulltext* in **Preferences/Plugins**.
2. Save your *Mercury API key* (~~apply for free [here](https://mercury.postlight.com/web-parser/)~~ Postlight has stopped providing new API key, you can continue using your current API key, read more [here](https://postlight.com/trackchanges/mercury-goes-open-source).) in the *Mercury_fulltext settings* under **Feeds** tab.
3. Configure for feeds under **Plugins** tab of the **Edit Feed** window (you can right click your feed to get there).

References
------------------------

* The plugin is modified based on [af_readability](https://git.tt-rss.org/fox/tt-rss/src/master/plugins/af_readability).
* [Mercury Parser](https://mercury.postlight.com/web-parser/).
