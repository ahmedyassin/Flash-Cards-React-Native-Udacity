# Udacity ReactND Project - Mobile Flashcards

The Mobile Flashcards app provides features similar to typical index cards used for studying. 
The app allows the user to create decks. Each deck contains a set of cards with a question and an answer.
The user can start a quiz for a given deck and evaluate themselves for correct or incorrect answers.
Users are given a score at the end of completing a quiz session.

A scheduled notification is shown everyday at 3:00 pm if the user hasn't attempted at least one quiz question for that day.

## Technical Specs

The app uses the following packages:

### Core:
- react
- react-native
- expo

### Navigation:
- react-navigation
- react-navigation-tabs


### Styling:
- react-native-elements

## Installation

1. You need to have Node.js, npm and yarn installed
2. Proceed by cloning or downloading the project as a zip
3. Extract and change directory to the project folder
4. Open your Terminal or Command prompt and type ```yarn install```
5. Then type ```yarn start```

## How to Run the App
The app has been tested on both Android and iOS physical devices 

- Install Expo https://expo.io/ on both Android and iOS
- All your devices (computer running the Metro Bundler, Android and iOS device) should be connected on the same local area network

### Android
1. Go to the Play Store and install Expo
2. Run Expo on the device
3. Scan the QR code available on the browser running the Metro Bundler
4. The Flashcards app should start 

### iOS
1. Go to the Apple Store and install Expo
2. Run Expo on the device
3. You can't scan the QR code on iOS, so you will have to either "Send link with email" or copy paste the link exp://192.168.0.109:19000 in Safari running on iOS
   - The network address may vary depending on your local area network setup so you might get something like exp://172.16.1.2:19000
   - Please look at the browser running the Metro Bundler, the link should be will be available under CONNECTION
   - Safari will ask permission to open the app in Expo: Open this page in "Expo"? Click Open
4. The Flashcards app should now start



### Decks

Decks view is also the home view, once you start the app you get the default Decks view. 
The first time you run the app, you will get 3 decks created by default:

- React
- JavaScript
- HTML and CSS

Feel free to delete these decks or create your own.

Every deck has a unique color based on an algorithm that creates a color value based on the text provided.

### Add Deck


You can create your own Decks by touching the Add Deck tab. 
Once a deck is created you are redirected back to the Decks view where you can see your freshly created deck.

#### Validation


Two validation checks are performed:
- Checks for empty values, deck title is required
- Checks for unique titles, deck title with an existing value cannot be created

### Individual Deck



Clicking on deck from the decks listing view shows the individual Deck view.

Here you can:
- Add a card to the deck
- Start a quiz
- Delete a deck

### Add Card to Deck


A deck card is the equivalent of the flash card or index card used for studying or exam preparation.

A deck card consists of:
- a question
- an answer

#### Validation


A simple validation is performed so that both question and answer fields have to be filled in.

### Quiz


A quiz can be started on any deck as long as there is at least one card.
The quiz will run through all the cards in the deck. 


The user can flip a card to check the answer and mark whether it was correct or not.

### Quiz Result & Score

The quiz result with the score is shown when the user has gone through all the quiz questions.

### Delete Deck

The user can delete a deck anytime. Deleting a deck will also delete all the questions in the deck.
