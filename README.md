# Instagram Focus — Android prototype

This prototype is designed as a focus layer for the official Instagram app rather than a replacement social network.

## Intended behavior

- Detect Instagram as the foreground app.
- Cover the lower navigation area so Reels/Explore navigation is not directly usable.
- Detect a selected Reels surface through the accessibility UI tree.
- Replace the visible Reels surface with a full-screen motivational message.
- Consume touches in blocked areas.
- Use white/near-black empty-space colors based on the device's light/dark UI mode.

## Important limitations

This is a prototype, not a guaranteed production-ready Instagram compatibility layer.

Instagram can change its accessibility tree, labels, hierarchy, or navigation. The detector therefore needs testing against the current Instagram build and additional fallback rules before release.

Google Play distribution also requires compliance with Google's Accessibility API policy, disclosure/consent requirements, and other applicable policies. Do not ship by falsely declaring the app to be an accessibility service for people with disabilities.

## Build

Open this directory in Android Studio and build the `app` module.

Then install the APK and enable:
Settings → Accessibility → Installed apps → Instagram Focus

The app intentionally requests no Instagram login and does not implement private Instagram APIs.
