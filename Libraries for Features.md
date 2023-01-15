# Libraries for Features

We need a few different functionalities in the app. Here, we'll note down the appropriate libraries for each feature

## 1. Calendar Bookings
Calendly is the perfect solution for this. As long as each user has a Calendly link, we can simply [embed their calendar](https://help.calendly.com/hc/en-us/articles/223147027-Embed-options-overview?tab=general).

## 2. Collaborative Whiteboard
As a first step, we can simply provide a link to a whiteboard app to both people. [Excalidraw](https://excalidraw.com/) seems like a great option
Eventually though, we'll want to embed an actual whiteboard into our platform. Thankfully, there appears to be an open-source [React library for Excalidraw](https://github.com/excalidraw/excalidraw) that can do the trick (don't know if it is collaborative or not, though).

## 3. Collaborative Editor with Syntax Highlighting
As a first step, we can simply provide a link to a Google Doc to both people.
Just as with the whiteboard, we'll want to eventually enable this in the platform itself. 

Something like the open-source project [Etherpad](https://etherpad.org/#) might work, although it seems to require us to deploy this to a 'host' machine, which will then serve the collaborative documents to our frontend through a [REST API](https://etherpad.org/doc/latest/#index_http-api). Might need some further research/work. 
Also, syntax highlighting doesn't seem to be supported natively - we may need to find an appropriate LSP implementation and integrate it into the code.
But they do have a plugin to enable audio/video chat (demo [here](https://video.etherpad.com/))!

## 4. Audio/Video Chat
TBD....
Kinda pinning all our hopes on EtherPad right now.
