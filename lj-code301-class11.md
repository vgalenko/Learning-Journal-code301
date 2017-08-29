# LJ Code 301 - Day 11

Today we were introduced to a Javascript library called Pages.JS. Its' purpose is to speed up the page load within a website. Instead of user waiting for each page to reload (which was done back in the day), page.js helps to speed up that process with a few methods that call on to local pages and instantaneously retrieve the files needed from server without reloading the browser.

Example:
```
page('/', index)
page('/user/:user', show)
page('/user/:user/edit', edit)
page('/user/:user/album', album)
page('/user/:user/album/sort', sort)
page('*', notfound)
page()
```
As seen in the page function the --> '/' alone will always refer back to the index page. If you want to target any file just add file name after '/'.
