# Polymer Test - Lluis Suros

## Summary
I used the Polymer Starter Kit template provide by `polymer-cli` a starting point. I think I could cover all the required points. Tests are provided in root/test. I had problems with Twitter calls and localhost so I built a mocked service.
 Hope you like it :)


### The displayed tweets are different from what you expected?
The service is mocked!

I had trouble trying to connect to Twitter to use their API. I created a Twitter account, an app, I got the credentials, and I could make requests with PostMan.
However I got blocked when trying to make the same requests from within my polymer code. I tried many things, used firebase autenthication, had CORS problems (maybe I should have connected via server-side). This was frustrating because I wanted to show that I can use <iron-ajax> but since the time was running out, I decided to create a `mock-twitter-service` that creates and retrieves twitter statuses just in the same way that Twitter API.

With this workaround I could continue. I think it was the right thing to do in this case.


### After getting the project get the dependencies

    bower update

### Start the development server

This command serves the app at `http://localhost:8080` and provides basic URL
routing for the app:

    polymer serve --open


### Build

    polymer build


### Run tests

This command will run
[Web Component Tester](https://github.com/Polymer/web-component-tester) against the
browsers currently installed on your machine.

    polymer test
