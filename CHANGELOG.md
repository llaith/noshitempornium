# Changelog
v1.5.5
- Fixed bug where NSE would not work on torrents.php after site update
- Fixed tag misalignment when using tag highlighter
- Add support for automatic updates

v1.5.4
- Fixed bug where script would not filter torrents on notifications page
- Fixed bug where options area would not appear in collages

v1.5.3
- Fixed a bug where NSE wouldn't work on torrents.php after a server-side HTML change

v1.5.2
- Clarified the explanations and reformatted the text in the management area

v1.5.1
- Fixed bug where a torrent would be hidden if an illegal tag was found after a whitelisted tag in the tag order

v1.5
- Added whitelist feature

v1.4.4
- Fixed bug where script didn't hide uploaders on top10
- Fixed bug where script wouldn't run on tag searches

v1.4.3
- More include/exclude changes, script should now run correctly on applicable collage pages whilst ignoring 
  torrent-pages with id or type parameters (torrent details, user seeding/leeching pages)
  
v1.4.2
- Fix bug where script didn't run on collage subpages

v1.4.1
- Convert includes to regex (PR [#1](https://github.com/ceodoe/noshitempornium/pull/1))

v1.4
- New feature: Hide by uploader name. This new feature allows you to specify usernames you want to hide 
  all uploaded torrents from, on all torrent browsing pages, and the Top 10 list. Collages are unaffected, 
  as they do not display uploader names on specific torrents. This feature works pretty much exactly like 
  the hide-by-tag feature, and hides a torrent if the username matches one on your list. At this time, you 
  cannot hide anon uploads. The list is space-separated, and case sensitive, which means that upper/lower 
  case of the username to hide matters. Please give this feature a go, and let me know how it works (or 
  doesn't work).

v1.3.3
- Fixed bug where toggle button would hide all torrents when clicked, when no illegal tags were found
- Slightly changed field design to be more fitting with default emp theme
- Made the Options button into an actual button
- Made code for button design more legible

v1.3.1
- Added matching of both .me and .sx domains
- Created GitHub repository for project

v1.3
- Major code restructuring and changes
- Added in-page taglist management (click [Options]), no more need for manually editing the script
- Removed ability to hide the toggle button, it is now required to manage tags
- Button is now always visible on applicable pages to enable taglist management when no torrents were hidden

v1.2.7
- Added toggling the toggle button by changing the toggleButtonEnabled variable's value
- Minor code changes

v1.2.6
- Now runs on individual collage pages

v1.2.5
- The script now also matches HTTPS, in case Emp ever implements SSL
- Toggle button will now show "torrent" instead of "torrents" when there's only one hidden element
