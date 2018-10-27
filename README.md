# YEN Changelog
Product updates, powered by our amazing community!

The goal withour `changelog` is to capture all of the work that we've done to build YEN, starting from the very beginning. This way we have not only a record of our collective accomplishments so we can celebrate our progress but also to increase the level of transparency into the process as we build.

In this way, our `changelog` is a bit different than more traditional ones because we're going to attempt to be a bit more specific with our notes (and definitely better than just a notice that reads: "*We constantly improve our application to provide better service to our users.*"...

We hope that you'll see many of the changes, improvements, bug fixes, and feature updates that you'll see are the **very ones** that **YOU** suggested! We love co-building with our community as it's just a better way of building.

Thank you!


















## Sprint 14

Goals for Sprint 14 were as follows:

## Sprint 13

Goals for Sprint 13 were as follows:

## Sprint 12

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









## Sprint 11

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