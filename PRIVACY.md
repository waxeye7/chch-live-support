# Privacy Policy: chch live

Effective: 15 October 2026

chch live ("the app", for iOS and Android) is a free app by Merlin Robin Stemmer ("I", "me"). It is an independent companion to [chch.live](https://www.chch.live). It is not run by Christchurch City Council, Metro or Environment Canterbury.

Privacy contact: stemmermerlin@gmail.com

This policy covers what data the app sends, who receives it, how long it is kept and how to ask for removal.

## What the app does not do

- No account or sign-in.
- No ads and no advertising identifiers.
- No analytics or tracking SDKs.
- No sale of data, and nothing shared for marketing.
- No in-app purchases. The app is free.

## Location

Location is optional. If you allow it, the app reads your device location in three places:

- **Near me.** The app sends your coordinates to `api.chch.live` to fetch reports near you. They are rounded to 3 decimal places, which is about 110 m. If you deny permission, or you are more than 60 km from central Christchurch, the app sends the coordinates of Cathedral Square instead.
- **Buses.** The app uses your position on the device to pick the nearest bus stop. Only the stop ID is sent to `api.chch.live`, not your coordinates.
- **Sent in.** When you take a photo, the app can attach a location pin. The pin is sent with 5 decimal places, which is about 1 m. See the next section for how it is stored.

The app does not save your location. I do not link Near me or Buses requests to your identity. Like any web service, `api.chch.live` receives your IP address and user agent with every request.

## Photos you send in (Sent in)

Sent in lets you take a photo with the camera and send it for review. There is no gallery picker.

**What is sent.** The photo, an optional caption of up to 140 characters, the capture time and, if available, a location pin. The original image can contain GPS data in its embedded metadata. The service can read the photo time and GPS from it, and it also receives the pin from your device location.

**What is stored.** For each photo the service stores the image, the caption, the exact coordinates, the capture and upload times, and the uploader's IP address and user agent. The IP address and user agent are kept for rate limiting and abuse review. They are not shown publicly.

**Screening and approval.** The service sends a resized copy of the photo to Google Cloud Vision SafeSearch. The copy has no caption, coordinates or IP address. Photos rated very likely adult or violent can be rejected automatically. A person approves every photo before it is public. There is no guaranteed response time.

**What is public.** Once approved, a photo can appear in the app and on chch.live. The public feed shows the photo, its caption, its suburb and its capture time. It does not show the coordinates, IP address or user agent.

**Reporting.** You can report a public photo from the app. The photo is hidden while a person reviews the report. A report record holds the photo ID, the reporter's IP address, the reason (if you give one) and the time.

**On your device.** The app keeps a local record with a reference to the camera image and the capture time, so your sends can appear in the Sent In list. Approved sends are removed from that list when they show up in the public feed. Rejected or removed sends can stay in the list until you clear the app's data, or until the app replaces them after 20 later sends.

## Rules for Sent in photos

By sending a photo you agree that:

- It is your own photo, taken by you.
- It does not show an identifiable person unless that person has agreed.
- It is not illegal, abusive, hateful, sexual or violent, and it does not infringe anyone's rights.

Photos that break these rules are rejected or removed. You can report any public photo you think breaks them.

## How long data is kept

- Rejected or removed photos, and their records, are deleted after 30 days.
- Pending, approved and flagged photos have no automatic expiry.
- Report records have no automatic expiry.
- Data held only on your device stays until you clear the app's data. You can clear it from the About screen.

## Deleting your data

To have a photo removed, or to ask what is stored about it, email stemmermerlin@gmail.com. Say roughly when you sent it and include the caption if you can. I will remove the photo and its record. Because there are no accounts, I can only find a photo from details like these.

## Other services the app contacts

The app is built on chch.live, and most content comes through `api.chch.live`. Some things go to other services. Each one receives at least your IP address and user agent, and the request itself.

- **Images on the Today wire.** Many images load directly from the publisher's or image host's own servers, not through chch.live. Hosts seen include news sites, Reddit, Flickr, Mastodon and iNaturalist image servers. Those hosts see the request.
- **Articles.** Tapping a headline opens the publisher's own page in an in-app browser. That site's own privacy policy applies to anything it collects. The app does not send your browsing history anywhere.
- **Nature sightings.** Opening a sighting contacts `api.inaturalist.org` with the observation ID.
- **App updates.** At launch, and about every 6 hours while the app is open, the app checks Expo (`expo.dev`) for updates. Expo sees your IP address, the app version and the update channel.
- **Bus stop data.** The app downloads bus stop and route files from `www.chch.live`.
- **Google Cloud Vision.** Used on the server only, to screen Sent in photos as described above. Google processes the resized copy on my behalf under Google's terms.
- **Links to other apps.** Map links and share buttons open other apps. The app sends nothing to them itself.

Content comes from chch.live and public sources, including Metro and Environment Canterbury realtime data (CC BY 4.0).

## Crash reporting

The app includes a crash reporting library, but it is switched off. It sends nothing. If it is ever switched on, this policy will be updated before that version is released.

## Security

The app talks to `api.chch.live` and my other services over HTTPS. Article pages opened in the in-app browser are the publisher's own and may use plain HTTP.

## Children

The app is not directed at children under 13. I do not knowingly collect personal information from children under 13. If you think a child under 13 has sent a photo, email me and I will remove it.

## Changes

I will update this page and its effective date if the app's data handling changes.

## Contact

Merlin Robin Stemmer: stemmermerlin@gmail.com
