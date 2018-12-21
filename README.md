# YEN Changelog
Product updates, powered by our amazing community!

The goal with our `changelog` is to capture all of the work that we've done to build YEN, starting from the very beginning. This way we have not only a record of our collective accomplishments so we can celebrate our progress but also to increase the level of transparency into the process as we build.

In this way, our `changelog` is a bit different than more traditional ones because we're going to attempt to be a bit more specific with our notes (and definitely better than just a notice that reads: "*We constantly improve our application to provide better service to our users.*"...

We hope that you'll see many of the changes, improvements, bug fixes, and feature updates that you'll see are the **very ones** that **YOU** suggested! We love [co-building with our community](https://github.com/yenio/changelog/wiki/3.-Our-CoBuilders) as it's just a better way of building.

Thank you!



## What is Your Software Development Lifecycle?

Okay, so, that's a mouthful, for sure! But, from here on out you might start learning a thing or two about the process of designing and developing great software! The `SLDC` (or also called the "Software Development Process") can look different based on the team and organization.

But what it is, essentially, is a framework of how ideas and concepts eventually become real software; it defines the tasks needed and the steps required to create working software. This often means developing a plan on how to develop, maintain, replace (or fix) the software. The **goal** is to not only produce something of value but also to help make the process, itself, better over time!

Our team specifically follows a plan that is broken down into 2 Week "Sprints" where we define the tasks we want to accomplish over those two weeks and also blocks out time to review the process itself.

Here's what this looks day-to-day:

### Week 1 (of 2)
- **Mon:** Day #3 of Sprint Cycle ("SC")
- **Tue:** Day #4 of SC
- **Wed:** Day #5 of SC
- **Thurs:** Day #6 of SC
- **Fri:** Day #7 of SC

### Week 2 (of 2)
- **Mon:** Day #8 of SC // Sprint Planning (Plan goals for next sprint, assign tasks)
- **Tue:** Day #9 of SC // Business Requirements (Decide technical solutions matching business logic with engineering requirements) // Code Freeze – "`Cinderella Deploy`" (changes allowed up until midnight PST)
- **Wed:** Day #10 of SC // Deploy to Development / Staging Branches
- **Thurs:** Day #1 of New SC // Master Deploy from Staging to Live // Sprint Retrospective // Goals for Next Sprint
- **Fri:** Day #2 of New SC

You'll notice that we start a new Sprint Cycle on the 2nd Thursday of the 2nd week. 

We plan on adding more context and material around our technical workflows over time but we hope you have learned a thing (or two) and find this type of thing not only interesting but perhaps even useful for your own projects (and those projects don't have to necessarily technical in nature)!

Without further ado... here's what our Sprints have looked like historically and the larger tasks that we attempted to work through!


***











## Sprint 18 (Dec 21 - Jan 11, 2018)

This Sprint is specifically 3-weeks long instead of the typical 2, given the holidays!


Goals for Sprint 18 are as follows:

- Continue working on Binance and Coincap integration
- Update Coinbase for new transaction workflow
- Admin Views for new Integrations
- API refinement for sending / receiving fiat exchange rate(s) 

... and more to be detailed soon!











## Sprint 17 (December 8 - 21, 2018)


Goals for Sprint 17 were as follows:

- Continue working on Binance and Coincap integration
- Update Coinbase for new transaction workflow
- Admin Views for new Integrations
- API refinement for sending / receiving fiat exchange rate(s)

Sprint 17 (and 18 and 19 most likely) are still heavily focused on getting our new integrations out and launched and so the next 2-3 sprint cycles will focus almost exclusively on those core elements.

This means that much of Sprint 17/18/19 will be a continuation of Sprint 16 in scope.

### Admin Views

- A new Announcement feature was built allowing us to communicate globally with our community
- Ability to create a new announcement with details (text, for now) with expiration dates
- Adding text editor for content creation
- Updating abuses
- Updating pagination on views
- Fixed 500 errors and error handling
- Adding internal search schema
- Results aren't displayed in the list when admin switches pages and uses Search
- Admin actions for posts, users updated
- Fix date picker
- Icon isn't uploaded for PACcoin currency when admin filters by symbol
- Change icon for Admin Actions tab
- NaN is displayed in row's range when admin clicks on Post link in Admin Actions tab
- New icon isn't uploaded on the page if previous icon was already uploaded in modal window
- Tags/mentions in the posts are displayed as HTML on the Posts page

### Binance and Coincap

- Working on updates and sync process for coin and token pairs
- Finalizing authentication to Binance
- Updating Coincap charting for backend and frontend
- Add cursor pointer to exchange tabs



### Updating Coinbase Workflow

- Fiat amount isn't displayed in Confirmation popup when user makes buy tx
- Buy tab isn't displayed when user makes buy tx and clicks on Start another buy
- Make selects for Buy/Sell tabs predefined on Coinbase tab


### API Refinement, Bug Fixes

- Refining chat sync for deactivated / deleted users
- Updating pagination
- Updating security protocol(s) for 2-factor
- User profiles should be clickable in messages
- Max URL length set (3,800 chars)
- Error handling improved, 500 / 422 errors on buy/sell
- Markup of buy/sell workflow update
- Remove restriction to change character in registration in nickname for user
- Incorrect parsing of mentions in posts
- More Blacklist entries updated into database
- Change date format in Created at column
- Metabase analytics built
- Unify send validations for blocked/deleted/non-confirmed users
- Request is sent and 422 error is received when user fills amount field and then deletes it
- Deleted user's avatar is displayed in Messages popup
- Post with livestream link does not appeared in Livestream tab
- `Follow:false` is received if user was following another user and was deleted














## Sprint 16 (November 24 - December 7, 2018)

Goals for Sprint 16 were as follows:

- Finalizing New Buy/Sell with Scalable Interface
- New Tokens Widget with Rates (Settings via User) with Coincap 
- Admin Panel Additions for New Coins (Coincap)
- Global Announcement Notification & Admin Management
- Binance Proof-of-Concept
- Bug Fixes and Improvements

We began Sprint 16 with some very, *very* large goals (e.g. tasks) in mind and we were unable to complete most of them in a single sprint cycle. This was expected so we'll continue to work on these items into `Sprint 17` [above](https://github.com/yenio/changelog#sprint-17-december-8---21-2018).

What we were able to do is knock out a ton of bugs, spend time optimizing the overall system, and making significant improvements app-wide.





### Admin Panel

- Special post type for announcements concepted, starting to build this and next sprint. Announcements will include `title` and `text` but nothing more, at least for now. Should be slightly different color and should be able to be closed by the user.
- Build out live deploy activities, work on docs and droplets
- Update admin / user features
- Shared functionality, search, and filtering
- Optimize abuses, blocked users, pages for deleted users
- New invitation codes for users by group or by individual
- Update blacklist
- Second page with search results is displayed when admin switches page and makes filtration on Users tab
- Add dropdown to Type column
- Update admin API, get UUID, add to JWT
- 500 error thrown on performing search via ID using non-numeric symbols
- Create Alerts for the different actions in admin
- Sometimes 500 error is received for login/adding invitations/search page
- Abuses: option to post, modal window
- Post isn't deleted when admin clicks on Delete icon in Posts tab
- Add 2 reasons to the filter on Abuses page
- Start_at and End_at with null are send in request when admin changes date in the row
- Handle error messages for admin panel
- URL doesn't fit in the column in Posts tab when user adds post with long URL
- Column's width isn't specified in styles - content is stretched vertically on Abuses page
- First list isn't displayed when admin makes search, switches the list and clears results
- Disable icons for deleted post in Posts tab
- Set max width for First, Last Name and Nickname columns on Posts page
- Change icon fo block/unblock users
- Add favicon to admin panel
- 422 error is received for api / posts / abuse when user chooses only reason in Report post popup
- Corresponding results aren't displayed when admin filters users by status/Unblock at
- Header's height is stretched when announcements are appeared
- Previous searching state is updated on Blacklist page when admin switches on another tab and return back
- Make chosen date highlighted in date picker

## Bug Fixes / Improvements

- Counter updating - 2 numbers by slash for Replays and Followers
- Moving buttons Edit profile and Settings
- Make tab text more obvious and shift to left
- Blocked user - profile view, a strip on the top with text: "Your account is currently `Deactivated`. Please contact support@yen.io if you have any questions."
- Page for deleted user
- Icon for new cryptocurrency BAT
- Widget trending topics: remove post counter under tags
- New 404 Page
- Distinguish the posts which are under processing
- Create icon for USD coin
- Tool tip for counters / button interactions with posts
- Incorrect displaying of date on profile screen
- Nicknames with "-" aren't clickable
- User mention in post is not redirects to his profile
- Disable email field in Settings for blocked user
- Login screen: notify user if cap locks is on while typing password
- Show what user's previous usernames were
- Add comment to transaction
- Rename "Broadcasts" to "Livestreams"
- Quick follow in popover
- Limit the characters in username
- Deleted user's avatar is displayed in Messages popup
- Display text about successful purchase above in popup
- Make user's avatar clickable on Messages and New Message popups
- Change text in New Message popup when user is not found
- Reduce height of exchange tabs and selects
- Change text on the strip and in popup for blocked user
- Fix a few login / logout issues




## Sprint 15 (November 9 - 23, 2018)

Goals for Sprint 15 were as follows:

- Finalizing Messages
- Finalizing Admin (Posts, Users, Abuse)
- Buy/Sell Redesign (Will start and finish in Sprint 16)

### Messages

- Ground-up Build using Node.js, MongoDB, Mongoose, Express, `Socket.io`, Docker, Ruby, etc., etc., etc....
- Build API for updating user, getting user info from backend, create users table

### Admin Panel

- Invitations page for admin
- Invitation Codes for Private Beta
- Blacklist
- Delete, Moderate messages
- Abuse management

### Bug Fixes / Improvements via BETA Testers

- Remove Intercom because it sucks
- Build Custom Metrics Views via AppSignal 
- Invalid currency format error on tx replay
- BAT hardcode (buy / sell)
- BAT hardcore (widget)
- Add USD Coin (buy / sell)
- Add USD Coin (widget)
- Prevent logging in / out while accessing `/login`
- Incorrect display of pictures in post
- Reduce size of notification
- Feed is refreshed when user opens any post and then closes it (for all filters except All tab)
- Post are not displayed for Global/MyFeed - All filter
- Author's profile isn't opened when user clicks on author's avatar/username from post's popup
- Comprehensive `db` backup in live via DO
- Use ruby-jemalloc docker image to reduce memory usage
- Add loader to image upload / post (`https://vue-content-loader.egoist.moe/`)
- Make hashtag in `TX` clickable
- Transactions are not displayed in Global =>Transactions filter
- Configure `DevOps` Channel in Slack
- YEN logos are not displayed in emails
















## Sprint 14 (October 25 - November 8, 2018)

Goals for Sprint 14 were as follows:

- Build the backend for Messages (Will start and finish in Sprint 15)
- Admin Panel (Will start and finish in Sprint 15)


### Messages

- Core functionality built-out (1-to-1 Direct Messages)
- Includes real-time notifications, awareness indicators, post/delete

### Admin Panel

- Add / Manage admins and moderators
- Blacklists for usernames
- Registration Codes (Individual and Groups with timeouts)

### Bug Fixes / Improvements via BETA Testers

- Impossible to repost a post
- Distinguish the posts which are under processing
- Placeholders for post with processing images
- Update the text in the field for different sorting
- Fix issue with 'Question Marks' in post (`?`)
- Impossible to add long link to the post

















## Sprint 13 (October 11 - 25, 2018)

Goals for Sprint 13 were as follows:

- Bug Fixes / Improvements via BETA Testers
- Add ZRX (Buy / Sell)
- Add 2FA Improvements
- Server Optimizations


### Add ZRX (Buy / Sell)

- Add ZRX to Transaction
- Add ZRX Icon to Widget

### Add 2FA Improvements

- Add 2FA Reminder Popup
- Should show after email confirmation
- If user selects "I'll Do This Later" we will remind them in 1 day
- If user selects "I'll Do This Now" then send them to settings page

###  Server Optimizations

- Make, improve background jobs
- Server stablity and performance upgrades

### Bug Fixes / Improvements via BETA Testers

- All the repeated tags within 1 post will be counted as 1
- Add icon ZRX to transaction
- Update trending tags widget
- Update transactions to handle new Coinbase responses
- [Text updates](https://beta.yen.io/yeneng/status/154109060747617) 
- More [text updates](https://beta.yen.io/yeneng/status/154109061993617)
- Increase size limit for uploading image files (5MB to 20MB)
- FE:Status for transactions in the field
- Tablet improvements: Fix scroll on iPad
- Search dropdown - arrows
- Shortcuts: Close modal windows with the `ESC` key
- Investigate 500 error due Coinbase verification
- Image operations refactoring
- Update typeahead API (If there are 2 hashtag options e.g. "btc" and "BTC" then typeahead API must return only latest option)
- Tags and mentions: Make them register-independent (case sensitive #yeniverse #YENIVERSE, they should be the same tag)
- Adding 2FA popup
- Update txn posts to parse crypto currency name as a tag
- Mentions and tags are not highlighted in repost comment
- Non-case sensitive nicknames
- Webpage is using significant memory (Mac)
- Tablet improvements: Logo in 404 redirect to feed
- Instant counter updating (not after page refresh)
- Handle different url forms in the posts
- Show counters in any case in any view (posts, tx, replay, fol)
- Tool tip for counters/ button interactions with posts
- Hardcode blacklist with nickname similar to core routes
- Live server setup. Release activities and fixes.
- SEO optimization - Parse manifest file for JS bundles to reuse frontend optimization
- Impossible to mention youself
- Like should be without delay
- Auto-expand links to .gif images
- The blocks with followers/followings aren't aligned by height in User Profile
- Disable graph on the Search page if the search is not related to currency
- 2FA:Connect timing of pop-up displaying and user id
- Show user info in bar on profile image hover
- Forbid access to adding phone for non-confirmed user
- Incorrect post ID - hide toast, show valid error in modal window
- 2FA: Popup is shown for guest user
- Terms of services: text update
- JS error in console on log out action
- Previous page isn't displayed when user clicks on browser's Back button from 404 page
- Incorrect redirect on profile image click from settings
- Registration form is overlapped with footer when user types invalid password and clicks on Continue button
- Smoother scroll for iOS
- Fix and improve background jobs performance + server stability
- Refresh feed by clicking on Global tab	
- Align name and nickname for repost with comment
- Update URL for TX History






## Sprint 12  (October 8 - 11, 2018)

Goals for Sprint 12 were as follows:

- Finalize BETA Server
- Onboard BETA users
- Don't freak out... enjoy the ride.
- Finalize Landing Page
- Build New Workflows for Support, Bug Fixes


### Fixes and Improvements

- Prototype for Notification receiver for multiple users (Binance)  
- Investigate 24h period exchange rates empty charts
- Chart should be adjusted to choosed cryptocurrency                                                                                                                               - UI: remember the choose coin in buy/sell                                                                                                                                         - 422 response is received for /api/posts/alex when user clicks on avatar in post's popup  
- Aggregation by likes moves up in the list of Notifications modal window although there is no new notification in aggregation 
- Continue button on Login form is disabled when user logs in right after 422 response is received for api/auth/login   
- Add retention policies to exchange rates influxDB series
- Update WEBPAK configs (for proper work of routes)                                                                                                                                - Notifications enhancements
- Likes / repost of transaction: Implement post opening in modal window
- Likes / repost post with video/broadcast: In notification body should be video preview (currently only link)
- Likes / repost  post with image - add image preview in notification body
- Comments: Implement post opening in modal window (preview in notification 
- Notification preview (drop down): Show only 5 last notifications 
- Mark all as read: Review implementation
- Images and gif are not displayed in mail in iphone mail client
- User could logged in with incorrect email format
- Settings: Change button to Enable Authenticator in 2FA block when user removes phone number in Security tab  
- Registration - fields validation
- Previews of avatars on Profile Page: Expand to larger version
- Small superficial design fixes: Name and username are not aligned in pop-ups
- Rename Broadcasts to Livestreams
- "YEN" banner is not stretch to full page size
- Incorrect behaviour of scroll in
- Display corresponding cryptocurrency in Buy/Sell popup when click on cart in Exchange Rates widget 
- Settings: Call "api/auth/check" returns "true" for email with space       
- TX History: User's own transactions are displayed in another user's profile when user changes the username in the URL
- Issue with scrolling the Likes List                           |
- Embedded transaction post is empty in notification block if user has notification about like added to his transaction
- Images in email are not showing
- Align pop-up messages to center, reduce size
- Double-check email confirmations
















## Sprint 11 (September 17 - October 5, 2018)

Goals for Sprint 11 were as follows:

- Setup Production Server
- 2FA Auth + Twilio
- Deploy Beta
- Big Bug Fix Party


### Setup Production Server

- Complete setup of production server
- DNS

### 2FA Auth + Twilio

- Refactor and test

### Deploy Beta

- Deploy with new CI
- DNS

### Big Bug Fix Party

- Over 125 issues covered. We rock.
- Browser test all-the-things

























## Sprint 10 (August 28 - September 14, 2018)

Goals for Sprint 10 were as follows:

- Direct messages (fix the known issue)
- Comments enhancement (expand, characters limit)
- Settings (backend)
- Search (add chart)
- Continuous Integration (CI)
- 2FA auth + Twilio
- Confirmation e-mail (Registration) e-mail mark up
- Google Analytics
- SEO optimization 



### Direct messages

- Continue to prototype models and API integrations


### Comments enhancement (expand, characters limit)

- Adding counter for character limitations
- Resizing input area

### Settings (backend)

- Finalize all backend for settings page

### Search (add chart)

- Original charting via Coinbase

### Continuous Integration (CI)

- Determine CI tools
- Create initial integrations with SDLC

### 2FA auth + Twilio

- Add phone
- On add, confirm via SMS via phone
- Disable 2FA if phone is connected: Allow deactivation sequence
- Settings: Enable or disable 2FA if you enter phone number

### Confirmation e-mail (Registration) e-mail mark up

- Add email markup on backend

### Google Analytics

- Frontend error handling
- User analytics
- Tracking and routing

### SEO optimization 

- Optimize app bundle
- Adding lazyload
- Add GZIP
- Hash to bundle to prevent browser cacheing












## Sprint 9 (August 13 - 28, 2018)

Goals for Sprint 9 were as follows:

- TRX History and Widget Last TRX status
- Transaction flow (buy/sell - not happy path - add validation)
- Notifications enhancement (required refactoring, post opening in modal window, 'mark all as read', etc.)
- Likes/reposts - expand on post preview
- Create plugins for messages
- UI improvements (add spinners for different API calls, profile cover image)
- Settings Page

### TRX History and Widget Last TRX status

- Tab includes the list of all transactions (sorting latest on the top)
- This is not a scalable solution (per Binance)
- Line: Icon / Transaction Details / Status
- Status: In Progress / Approved / Cancelled
- View by Default: All TRX from the latest on top, filtered by status (Created / in Progress / Approved / Cancelled)

Widget TRX:

- Displays the latest TRX with status
- After approval TRX should be displayed in widget for 30 seconds
- It will only show the latest TRX
- When the displaying TRX becomes approved we'll poll the API for udpated state
- Show more: User goes to TRX history page
 
Status Description:

- In progress: TRX committed and processing (via Coinbase)
- Approved: Final successful state of TRX
- Canceled: Final state of TRX is unsuccessful

### Transaction Flow (Buy / Sell, Add Validation)

- API investigation: Error messages
- Prepare designs for failures
- Workflow for user to oAuth into Coinbase on Buy / Sell or Replay

### Notifications Enhancement (Refactoring, post opening in modal window, 'mark all as read', etc.)

- Likes/repost of transactio: Implement post opening in modal window
- Likes/repost post with video/broadcast: In notification body should be video preview (currently only link)
- Likes/repost post with image: Add image preview in notification body
- Comment: Implement post opening in modal window (preview in notification)
- Notification preview (drop down): Show only 5 last notifications 
- Mark all as Read: Implementation is complete


### Likes / Reposts: Expand on Preview

- Design is not complete, although behavior is similar to Twitter
- When user opens post in preview (modal window) additional fields appear
- On Like or Repost: Opens modal window with all users who liked / reposted the post
- By clicking on icon (icons with users who liked my post): Goes to profile of user
- All users in the list of 'who liked / reposted' my post should be clickable

### Create plugins for messages

- Create API plugins for possible implementations (PubNub, Chat Engin)
- Move them to Vue
- Improve security

### UI Improvements

- Add loading spinners for different API calls

### Settings Page

- Account Info and Coinbase Account
- Coinbase: Show Name, Surname
- Change password, with error messages and saving mechanics 
- Add security: Phone number and 2-Factor Authentication
- Notification settings
- Privacy Policy: Empty page for now (text TBD)
- Forgot password
















## Sprint 8 (July 30 - August 10, 2018)

Goals for Sprint 8 were as follows:

- Direct messaging: Increase chat security
- Direct messaging: Delete messages, add time of message, load on scroll
- Widget Trending Topics
- Notifications: Aggregation and Filter
- Landing Page

### Direct Messaging: Increase chat security

- A new direct chat gives temporary permission to user; when permission expirese, they will not be able to access chat

### Direct messaging: Delete messages, add time of message, load on scroll

- Done

### Widget Trending Topics

- Execute against [design concept](https://www.dropbox.com/s/n8hxgrp8jyipjz3/trending-topics.png?dl=0)
- Dynamic for 12 hours, 5 most often used tags in posts
- Should update ever 1 hour, top 5 tags rotate out
- Chart: 12 points (1 points / hour)
- Arrows should compare the latest 2 inputs

### Notifications: Aggregation and Filter

The types of notifications are as follows:

- Likes user's post
- Repost of user's post
- Replayed transaction
- New follower
- Comment on user's post (without aggregation)
- @mentions user

The counter for notifications should aggregate by type (for example there are 3 likes and 1 comment, the user should get 2 notifications total)

### Landing Pagepage enhencement (left panel: total transacted value, search, trending topics)

- Original [sketch](https://www.dropbox.com/s/py1ypp04m712b5x/IMG_2676.jpeg?dl=0)

Left panel: 

- Total transacted value ($ equivalent of all buy/sell operations)
- Total replays (amount of all replays of transactions)
- Total subscribers (amount of all registered users)
- Search should go to search page on input
- Trending topics: The posts with max amount of likes within 2 last days

Right panel:

- Login
- Registration







## Sprint 7 (July 16 - 27, 2018)

Goals for Sprint 7 were as follows:

- Direct messaging (text only)
- Autotests: Creation of all types of posts and reposts
- Refactoring of reposts
- Search (Algolia, backend)
- Tags (Frontend)
- Mentions (Frontend)
- Binance Prototype for Notification Receiver for Multiple Users



### Direct Messaging

- Text only
- Based on initial [lofi wire](https://www.dropbox.com/s/ppo8r247drm6pg9/messages.png?dl=0)


### Autotests: Creation of all types of posts and reposts

- Automated testing of post creation, reposts

### Refactoring of reposts

- Data is quite large and unstable
- Goal of refactor: Detect common structure in all types of posts and divide large functions into smaller, more modular buildsN

### Search (Algolia, backend)

- User enters text in search field, should should suggestions
- User can tap suggestions to auto-complete (shortcut)
- List suggestions matching username / surname or nickname
- Search results show people and posts
- Filters for search results in top menu

### Tags (Frontend)

- Done

### Mentions (Frontend)

- Done

### Binance Prototype for Notification Receiver for Multiple Users

- Done... looks legit af.










## Sprint 6 (July 2 - 13, 2018)

Goals for Sprint 6 were as follows:

- Comments
- Responsive layout for tablet
- Dislike removing
- Pagination for posts (infinite scroll)
- Tags (in posts)
- Repost functionality
- SEO optimization (finalizing)
- Binance investigation
- Bug fixes


### Comments

- User (logged in) can comment on any post or transaction
- Clicking the "Comment" icon should open modal window
- "Reply" adds @username, comma, then space and text
- Comments are limited to 300 characters like posts
- Comments have infinite scroll

### Responsive Layout for Tablet

- First designs for tablet (e.g. iPad) for 1024px

### Dislike Removing

- Done


### Pagination for Posts

- Infinite scroll built out, a'la Twitter

### Tags (in posts)

- Done


### Repost Functionality

- Like [this](https://www.dropbox.com/s/j1vc7fl2sup87z7/repost.png?dl=0)!


### SEO Optimization (Finalizing)

- See previous sprint

### Binance Investigation


### Bug fixes

- Slay them bugs, yo.
- Too many to mention...









## Sprint 5 (June 18 - 27, 2018)

Goals for Sprint 5 were as follows:

- Add Likes
- Post preview (in modal window, comments)
- SEO accessibility of post pages + OpenGraph
- Delete user's post
- Cache images in CDN
- Prototype Binance integration
- Permission management system     
- Bug fix: Buy / Sell posts and their replays are not displayed correctly
- Bug fix: Image uploading is not working properly



### Add Likes

- Like / Dislike functionality for all posts
- Add Like / Dislike counter

### Post preview (in modal window, comments)

- Click on post area / body, the current post should open in modal

### SEO accessibility of post pages + OpenGraph

- Done

### Delete user's post

- Done


### Cache images in CDN

- Review CDN integrations (e.g. Cloudinary)

### Prototype Binance integration

- Test API calls and response(s), review workflow and prepare recommendations on how YEN can support Binance

### Permission management system     

- Done

### Bug Fixes 

- Buy / Sell posts and their replays are not displayed correctly
- Image uploading is not working properly








## Sprint 4 (May 29 - June 14, 2018)

Goals for Sprint 4 were as follows:

- Profile of users (frontend)
- Global feed (recent posts of all users)
- Replay transaction
- All type of my posts feeds (posts, images, video) via profile
- Follow / following functionality

### Profile for Users

- User can go to profile of other users only through URL in format `yen.io/username`
- Displaying of page: `yen.io/username`

### Global Feed

- The feed is the same as My Feed with the same filters, the difference is that Global Feed (2nd column) contains the recent posts of all users in the system.
- Prioritization of posts - only by creation time
- Add cacheing for posts with transactions (backend).
- Indicate in transaction the difference between 'buy' and 'sell' transactions

### Replay Transaction

- Replay will repeat logic of Buy / Sell
- Statistics in transaction
- Transaction speed / rate
- Add API for Buy / Sell for account

### All Type of My Posts Feeds

- Following: Should be displayed on profile block
- Following management on User profile
- Display status of other user (follow is true or false) when current user goes to another user's profile
- API actions for follow / unfollow
- List follows / following of current user in profile 

### Follow / Following Functionality

- User profile should display 2nd colum with only current users posts
- Filter of posts via profile
- Posts: Only text posts
- Reposts: The reposted posts (all types) and transactions
- Media: The posts with URL preview, images, video, livestreaming 
- Transactions and Replays: Show the `parent` transactions and replayed transactions









## Sprint 3 (May 10 - 23, 2018)

Goals for Sprint 3 were as follows:

- Currencies in exchange rates (refactoring)
- Add basic auth for alpha
- Coinbase webhook notifications (for buy/sell transactions)
- Messaging (+invest) - realtime post refresh after creation - for current user
- Vuex
- Add posts manually, images
- Buy/sell via Coinbase from Yen
- Profile for other users (API, layout on frontend)

### Currencies in Exchange Rates (refactoring)

- Should look like [this](https://www.dropbox.com/s/4hdq7etkfylnatv/widget-exchange.png?dl=0).
- Supported currencies for now: USD, EUR, GBP, CAD, CNY

### Add Basic Auth for Alpha

- Looks like [this](https://www.dropbox.com/s/71zrlenkm19i2uk/yen-sign-in.png?dl=0).

### Coinbase Notifications

- As an authorized user via Coinbase, my transaction will be visible to others and they can receive notifications about user's activity.
- As an authorized user via Coinbase, data of my transactions will be save in YEN DB.
- As a logged-in user, I can filter transactions by type: Buy / Sell
- As a logged in user, I can see transactions of the authorized users via Coinbase in the 2nd column of the feed.
- As abn authorized user, I can buy / sell via Coinbase from YEN.

### Messaging

- Continue prototyping

### Vuex

- Add Vuex library to front-end, allowing better cross-dependent utility.

### Add Posts

- Displaying of images in 2nd column.
- Image (full size) should be opened after user clicks on its preview.
- Image uploader from folder: Add custom files features with only-image extensions.
- Backend will send list of images with 2 sizes: Original and preview.
- Sizes of previews will be always same.
- On frontend the images (1-4) will be displayed.
- Published posts cannot be edited.

### Buy / Sell via Coinbase

- Completed. :unicorn:

### Profile for Other Users

- User can go to profile of other user only through URL in format `yen.io/username`
- Displaying of page: `yen.io/username`













## Sprint 2 (April 26 - May 8, 2018)

Goals of Sprint 2 were as follows:

- Creation / Displaying of video posts (static video file and streaming)
- User Profile
- Coinbase Webhook Notifications
- Exchange Rates Widget
- Messaging Prototype

### Create / Display Video Posts

- User should be able to create a post with a URL to a video site (YouTube, Vimeo) for both on-demand and livestream (YouTube-only).
- Post should be displayed in the 2nd dynamic column on the feed.
- To embed videoPost should be displayed in the 2nd dynamic column on feed.

### User Profile

Profile basic screen contains the [following fields](https://www.dropbox.com/s/j7pwdncjuwwaqt5/3-0-1-profile.png?dl=0):

- Update photo (optional)  
- Name (mandatory)
- Last name (mandatory)
- Full description (optional)
- Website (optional)

Validation for fields:

- Photo: size limit: UYp to 5.0MB
- Name and Last Name fields: Minimum of at least 1 symbol or character
- Full description: Up to 100 characters
- Website: Should contain `http:`or `https:`, text / dot / text
- Should be implemented with a loader for images (file extensions are jpeg, gif, png, tiff, and bmp)

### Coinbase Webhook Notifications

- Authorized user via Coinbase oAuth
- YEN should receive notifications about user's activity
- Display transaction in second dynamic column
- Save all transaction data in DB with ability to filter / sort (buy / sell)
- Enable Buy / Sell actions via Coinbase from YEN

### Exchange Rates Widget

- Design a widget that shows current pricing of coins / tokens

### Messaging Prototype

- Complete a concept / prototype for internal messaging using off-the-shelf APIs (e.g. PubNub)















## Sprint 1 (April 11 - 25, 2018)

The goal of this first (!!!) sprint was to identify our core architecture and establish baseline goals for MVP, including:

- Core Architecture 
- Authorization + Registration 
- Create and Display Text (with or without URL post)
- Design a 3-column feed where the middle (2nd) column is dynamic (updating) with text and/or URL post 
- Coinbase oAuth Test

### Initial Concepts

- [Concept 1](https://www.dropbox.com/s/www9zykc22ymu6d/concept-1.JPG?dl=0)
- [Concept 2](https://www.dropbox.com/s/bm0v034xi8cj110/concept-2.jpg?dl=0)
- [Concept 3](https://www.dropbox.com/s/wt7h2tck9vh9o1g/concept-3.jpg?dl=0)
- [Concept 4](https://www.dropbox.com/s/4zktb3nmioiwpk9/concept-4.jpg?dl=0)
- [Schema](https://www.dropbox.com/s/gaap2lpovv7s30p/yen-schema-draft.jpeg?dl=0)

### Authorization & Registration

Authorization/registration screen should look like [this](https://www.dropbox.com/s/5mgd40h0wc2picb/0-0-0_register.png?dl=0):

For MVP: Registration only via email (in the future we may have google, fb, twitter, bitcoin pub accounts)

### Create and Display Text

- Only text posts and posts with URL will be accepted.
- User can add new post ([screenshot](https://www.dropbox.com/s/9qtulwn9fznwl4w/2-post-two.png?dl=0))
- Upload up to 4 images (via drag-drog or upload)

### 3-Column Design

- 3 colums where the 2nd column is dynamic with posts. All other columns will be empty.
- LoFi [concept](https://www.dropbox.com/s/l3naboqz83hwimz/1-0-0_feed.png?dl=0).

### Coinbase oAuth Test

- US-Only: User needs to be able to connect to Coinbase via oAuth (YEN makes backend call to Coinbase API on behalf of user).I
- [Success](https://www.dropbox.com/s/zjcjwcx5jhwpa9s/success.png?dl=0)!  

<3
