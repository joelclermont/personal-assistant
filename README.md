Personal Assistant
==================

This application provides a voice or SMS-based interface to your calendar data. It uses [Twilio](http://www.twilio.com/) to do the heavy lifting for the voice/SMS interaction. Best of all, it does not require you to make your calendar public.

Possible uses
-------------
* Tell a caller if you are out of the office or just busy/unavailable.
* If you're at an appointment, tell the caller how long you'll be gone.
* Tell the caller specifically where you are so they can join you (social events)
* Provide them a context-specific alternate way to contact you (for example: if you're on a boring conference call, recommend IM/SMS)

Considerations
--------------
Calendar data can be quite sensitive, so the application will be configurable to only integrate with the specific calendars you wish. In addition, these calendars may require authentication (not public). Finally, there may be individual items on a calendar that you want to be more available or less available. This can be handled with event metadata or simple title modifications.

Since we're dealing with times, we'll have to handle time zones as gracefully as possible. At a minimum, we should announce the time zone along with any spoken times. To get fancier, we could integrate with an address book and use that information to set a more appropriate time zone for a specific caller. Even in these cases, though, the time zone should be spoken to avoid confusion.

Other ideas
-----------
The caller ID information can be used for additional context. For example, you might want a friend to know you left early for a round of golf and invite them to join you, but maybe not a client/boss. Or if the person calling you is the same person you are meeting with, you can let them know you are already en route and connect them to your mobile.

If you have any other ideas, feel free to suggest a feature.
