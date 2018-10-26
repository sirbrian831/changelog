# YEN Changelog
Product updates, powered by our amazing community!

The goal withour `changelog` is to capture all of the work that we've done to build YEN, starting from the very beginning. This way we have not only a record of our collective accomplishments so we can celebrate our progress but also to increase the level of transparency into the process as we build.

In this way, our `changelog` is a bit different than more traditional ones because we're going to attempt to be a bit more specific with our notes (and definitely better than just a notice that reads: "*We constantly improve our application to provide better service to our users.*"...

We hope that you'll see many of the changes, improvements, bug fixes, and feature updates that you'll see are the **very ones** that **YOU** suggested! We love co-building with our community as it's just a better way of building.

Thank you!

















## Sprint 16

## Sprint 15

## Sprint 14

## Sprint 13

## Sprint 12

## Sprint 11

## Sprint 10

## Sprint 9

## Sprint 8

## Sprint 7

## Sprint 6

## Sprint 5

## Sprint 4

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