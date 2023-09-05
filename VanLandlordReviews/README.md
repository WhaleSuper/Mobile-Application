# CS5520 Mobile Application - Assignment 3


## App: VanLandlordReviews


## Group 5 team members: 
- Yang LI
- Youjing SHEN (Simona)


## Demo:
demo link: https://youtu.be/wihyv3EsQr4


## Iteration 1
## Submission repo branch: Iteration1


## Data Structure Design:
- To complete our design, We apply 3 collections: review, comment, and user.
- Collection user: contains userId, nickName, reviewId, commentId, in which reviewId and commentId link to collection review and comment separately.
- Collection review: contains id, address, postalCode, rental, term, city, description, comments(array), createdBy, in which comments and createdBy link to collection user and comment separately.
- Sub Collection comment under collection review: contains id, content, reviewId, userId, in which reviewId and userId link to collection review and user separately.


## Project work allotment (Iteration1):

Both:
1. App functionalities and structure design.
2. Styles and layout improvement.
3. Repeated tests.

Yang:
1. firebase-setup.js
2. firestore.js
3. helper: color.js
4. ReviewList.js
5. AddReview.js
6. AllReview.js
7. FavoriteReview.js

Youjing:
1. SingleButton.js
2. PressableButton.js
3. PressableButton2.js
4. CommentList.js
5. ReviewDetails.js
6. UpdateComment.js
7. Me.js
8. Main.js


## Iteration 2
## Submission repo branch: Iteration2

## Functionality update description
1. Add Authentication (Youjing)
2. Add Camera and Gallery -- users can now take photos or upload images from local gallery to their new posting reviews (Yang)
3. Add Location -- users can now choose their current location or any target location when posting their new reviews(Yang)
   
## Update existed functionalities:
- Add likes, count likes and favorites for comments and reviews (Yang)
- Redesign Detail screen and comment components (Youjing)
- Add new fields for users when posting new reviews (Youjing)
- Applying dropdown and other buttons to diversify functionalities (Yang)
- Fix UI of components (Youjing)

## Prepare for Iteration3
- (See Note)

1. Add external API (walk scores API decided).
2. Add Notification functinality.
3. Modify UI of various screens.
4. Optimize style design.

## Iteration 3
## Submission repo branch: Iteration3

## Functionality update description
1. Add External API -- walkscore in Detail screen sourcing from https://www.walkscore.com/ (Yang)
2. Add Notifications -- both local notification and push notification. (Yang)
3. Modify UI and fix warnings (Youjing)

## Update existed functionalities:
1. Now new users will receive a local notification when they stay at Me screen for 5s, reminding to post their own reviews.(Yang)
2. Now users will receive a push notification if their posted reviews are commented by others.(Yang)
3. Now users can find a property "walkscore" sourcing from an external API. If address, postal code, and city doesn't match, it reminds "Not Found".(Yang)
4. Now KeyAvoidView is added to make users more comfort.(Youjing)
5. Now the address users click on google map will be automatically updated to textInput address. Users don't have to always manually input address.(Yang)
6. Now some UI changes for beauty.(Youjing)
7. Now warning of depreciated properties when uploading images from local gallery is fixed.(Youjing)

