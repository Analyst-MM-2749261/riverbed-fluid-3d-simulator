# Privacy

## Summary

The public offline release is a self-contained HTML application. It does not
require an account and is designed not to send application data to a server.

## Persistent storage

Version 51 does not use:

- `localStorage`;
- `sessionStorage`;
- cookies;
- IndexedDB;
- a service worker or application-managed persistent cache.

Parameters, selected tabs, pinned controls, recent controls, fluid state, and
riverbed state exist only in JavaScript and GPU memory while the page is open.
Reloading or closing the page resets them.

A browser or operating system may retain the downloaded file or normal browsing
history according to its own settings. That behavior is outside the
application.

## Device orientation and vibration

For visual interface effects, the application may:

- request device-orientation permission through `DeviceOrientationEvent` on
  supported mobile browsers;
- use a short vibration through `navigator.vibrate` for touch feedback.

These features are optional, may be denied, and are not used to identify the
user. The application contains no code that transmits orientation values to a
network service.

## Network behavior

Repository-root `index.html` contains runtime libraries and CSS inline. It has
no external script, stylesheet, image, font, form endpoint, analytics endpoint,
or application API endpoint.

Some bundled libraries contain inert documentation, namespace, or error-help
URL strings and unused networking functions. Their presence does not by itself
initiate a request. Release testing should still confirm behavior with the
browser Network panel while offline.

The file under `source/` is a development/reference version and deliberately
loads dependencies from CDNs. It is not the offline release.

## Personal information

Static review found no account, analytics, advertising, upload, remote logging,
geolocation, camera, microphone, email address, API key, access token, or
application-data submission feature.

## Future changes

If a future version introduces network access, analytics, uploads, persistent
storage, or additional sensor access, this document must be updated and the
release audit repeated before publication.
