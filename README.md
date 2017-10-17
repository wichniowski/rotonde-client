# Rotonde/client

**Rotonde** is a decentralized social network based using an equally *decentralized* application. The two parts of the application are :

- [client](https://github.com/Rotonde/client), the core of the application.
- [user](https://github.com/Rotonde/user), the user files, settings and customization.

The client, or *Rotonde Core*, is the client base is what contributors need to fork to make improvements on the inner systems of the application. This separation allows for a simplier onboarding and updating flow, where the latest client revision will be seeded automatically, while the [user](https://github.com/Rotonde/user) source is all that any simple user need to maintain.

## Setup

This setup is only temporary until every has migrated to the decentralized application paradigm. Then, joining Rotonde will be as simple as clicking **Fork**. If you already have a `portal.json`, copy/paste it into the user repo.

- Clone both repositories in your `~/Sites`
- Create two sites using the [Beaker Browser](https://beakerbrowser.com) and point them to the user/client repositories.
- Update the user/index.html file with your client site hash, found in the beaker url navi.
- Update the client/dat.js with the client site hash, and the client/dat.js with the user site hash.
- Share your `dat:` url with people, and past theirs to follow them.
- Enjoy!

## Commands

- `dat://000` will follow a portal.
- `undat://000` will unfollow a portal.
- `filter @neauoire` will show your mentions.
- `clear_filter` will clear the filtered feed.
- `edit:name Some_name` will change your display name.
- `edit:desc Some_name` will change your display description.
- `edit:site Some_name` will change your display site.
- `edit:0` will edit your first entry.
- `delete:0` will delete your first entry.

## Runes

- `@` means you seed eachother.
- `~` means that they do not see you.
- `$` means that they are a service or a bot.

## Icon

To change your display icon, update the SVG file located at `media/images/icon.svg`. The icon should be a square file for it to display properly. Keep it small. If you update your svg manually, don't forget to go to Library->(Your Rotonde Site) and press Review Changes -> Publish, otherwise your changes wont be seen by anyone!

## Rich content

- `TEXT >> MEDIA_NAME.jpg`, will connect a media filename from `/media/content/MEDIA_NAME.jpg`.
