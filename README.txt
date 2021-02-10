https://tableau.github.io/webdataconnector/docs/wdc_oauth_tutorial.html

When a user clicks the Connect to Foursquare button, y
our code redirects the user to Foursquare, where the user can sign in. 
After the user signs in, Foursquare redirects the user back to the local web server with an authorization code. T
The web server takes the authorization code and adds the client secret in a request back to Foursquare 
to get the access token that will be used for making requests for data. 
Foursquare sends the access token back to the web server. 
The web server saves the access token in the browser cookie, so that the client code (your web data connector) 
can retrieve it. You’ll add code to retrieve the OAuth access token from the browser cookie.