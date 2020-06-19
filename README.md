![screenshot](https://i.ibb.co/t2dVZ3y/Capture.png)

Jackett Metasearch (probably need to figure out a better name) is a modification of Web Interface of [Jackett](https://github.com/Jackett/Jackett) to only display the window which shows up when "Manual Search" button is clicked. This allows for the operation of Jackett like a meta torrent search engine like torrentz.

I have modified Jackett's HTML,CSS,JS and made following changes:
1.	Load the manual search automatically when the page is opened.
2.	Hidden “DL Factor”,”UL Factor” and “Grabs” from the search result table using CSS
3.	Remove X button and Close button from manual search
4.	Made the search box a bit bigger and rounder
5. Disabled the event which triggers when backdrop is clicked.

What more should be done?
1. Administrator login which leads to regular jackett interface
2. The search results should be displayed better on mobile
3. Category buttons like on many torrent sites
4. Search result should be displayed on a different window/page.


I really needed a way to search torrents from public trackers; I have previously setup a DHT Scraper on my VPS but that just scrapes a ton of garbage. NZBHydra can be used with Jackett for searching content on torrent sites but it adds another unnecessary step as Jackett already has Manual Search built in.

 I would greatly appreciate some help with making this look better and prevent anyone unauthorized from changing the indexers as the Javascript isn't changed at all (just not being executed or displayed).
 
That said, it does indeed “work”, you will have to setup all the indexers normally and then modify the html,css,js files.
