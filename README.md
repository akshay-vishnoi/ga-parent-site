# ga-sites

There are 2 rails sites in this repository. I have used official GA [documentation](https://developers.google.com/analytics/devguides/collection/analyticsjs/cross-domain#iframes) to test cross-domain tracking of events with iframes.

Setup:

1. `bundle install`
2. Run `rails s -p 3000`. Run both sites on different port. You can see the GA code on root page of both applications.
3. Setup ngrok for both sites.
4. Add ngork URLs in GA admin. Put parent site URL in property settings. And put both URLs in referral exclusion list
5. Change iframe site URL in HTML as well. For JS and HTML of root page checkout `app/views/layout/application.html.erb`.
7. Change UA id provided from your GA account in JS.
8. Post the parent site URL in facebook and then visit the page. 
