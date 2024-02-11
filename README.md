### Notice: 6 Feb 2024

Unfortunately I started having issues with my hub replicator after the unprecedented growth since the launch of Frames due to hardware constraints. Working on syncing the new replicator but still having trouble and haven't had the time to fix unfortunately so my instance opencast.stephancill.co.za is down for now.

You are obviously free to (and I encourage you to) run it locally. Opencast supports the legacy replicator (check out the hub-monorepo around November last year) and the new replicator (hub-monorepo/apps/replicator) so you can use either. Running the replicator is quite challenging - please share your findings if you manage to successfully sync.

# Mach5cast implements Opencast(fork) The Opencast repo cloned to Mach5.cast on 12/11/2024 
# (GOAL -> clone Farcaster and launch on PulseChain CHAINID: 369, set-up HUB - clone software, Launch Mach5 Wallet w/ Farcaster features)

A fully open source Twitter flavoured Farcaster client. Originally a fork of [ccrsxx/twitter-clone](https://github.com/ccrsxx/twitter-clone).

The goal of this project is to provide a reference implementation of a Farcaster client in order to make it easier for developers to explore their ideas without having to start from scratch.

It only depends on the reference Farcaster postgres indexer and optionally a hub for submitting messages.

## Development 💻

### Farcaster Replicator

This project depends on the reference Farcaster PosgreSQL indexer. Follow the instructions at [replicate-data-postgres](https://github.com/farcasterxyz/hub-monorepo/tree/main/apps/replicator) to set up an instance.

### Local

1. `yarn`

1. Copy the `.env.sample` file to `.env` and fill in the database connection details.

1. `yarn dev`

## Todo

- [ ] Feed
  - [x] Reverse chronological feed
  - [x] Pagination
  - [x] Number of likes, comments, and reposts
  - [ ] Recasts
- [x] Cast detail
  - [x] Number of likes, comments, and reposts
  - [x] Paginated replies
- [x] User profiles
  - [x] Casts
  - [x] Casts with replies
  - [ ] Media
  - [x] Likes
  - [ ] Edit profile
- [x] Auth
- [x] Engagement actions
- [x] Post creation
  - [x] Text only
  - [x] Media
  - [x] Mentions
  - [x] Embeds
  - [x] Topic
- [x] Post deletion
- [ ] Search
  - [x] User
  - [ ] Topic
  - [ ] Posts
- [x] Channels (now called Topics)
  - [x] Channel detail
  - [x] Channel discovery
  - [ ] Index channels
- [x] Fix mobile layout
- [ ] Rebrand
  - [x] Renaming (casts -> tweets, etc)
  - [x] Images
  - [ ] Code
- [x] Notifications
  - [x] Badge counter
  - [x] Notifications page
- [ ] Optimize
  - [ ] DB queries
  - [ ] Bandwidth

...

## Tech 🛠

- [Next.js](https://nextjs.org)
- [TypeScript](https://www.typescriptlang.org)
- [Tailwind CSS](https://tailwindcss.com)
- [SWR](https://swr.vercel.app)
- [Headless UI](https://headlessui.com)
- [React Hot Toast](https://react-hot-toast.com)
- [Framer Motion](https://framer.com)
