# Viewers

The admin, customer admin, and website clients can probably overlap like 80%

## Admin

We'll need an admin client for things like

* setting event information (filters, branding, tweet-settings)
* deleting particular gifs
* tracking stats?

## Customer Admin

We might want an admin client for customers with things like

* promoting particular gifs to their twitter
* tracking stats?
* deleting particular gifs

## Website

Of course, there's the main booth-display website at gifbooth.co

# Booths

Thanks to the growing reach of javascript, one codebase can target web, ios, android, mac, and windows. 

Once we have a booth, any future event can target that booth. Sell the whole package (website, app, physical booth), create (or choose) some filters, and deploy to *all of those booths* in seconds.

## Openframeworks-booth (C++)

This is the booth we already have, and it could be modified to work with the new server (except filter management) pretty darned easily [think hours not days. A freebie once the server is up].

## Web-booth

A kiosk-mode chrome window (rather than a native app) is the best solution going forward for desktop (mac-mini). 

By making web-booth, we'll also have made:

* a saleable online branded gifbooth-at-home experience
* an image processor that will run on the server
  * (which in turn makes something like an mms-booth super trivial (a day, tops)

## Mobile-booth

This booth could be used for putting an iPad on the wall at an event, or for selling an event-branded instagram-like booth app.

React-native can generally target android and ios at the same time with minimal extra effort. Right now, the graphics capabilities of react-native on Android aren't quite where we want them, but they will be within a few months.

## Bullet-time-booth

This is actually a pretty straightforward one 'cuz it's so specialized. It wouldn't take more than a day to set up, but would require a lot of hardware setup. Get *n* raspberry pis with camera, print some proper cases, and have one pi coordinate the others. The shutter could be a button on a website/phone/wall/anything.

