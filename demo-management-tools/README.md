# Google Play Games Services Management Demo #

This demo console shows you how to use the Google Play Games Management API to
manage and test Google Play Games Features.

## Installation ##

Tried to fix all console errors by using [Web Components](https://www.npmjs.com/package/@webcomponents/webcomponentsjs) and [Polymer 3](https://polymer-library.polymer-project.org/).

1. Install Node.js and npm. Install them by [nvm](https://github.com/nvm-sh/nvm) is suggested.

`nvm use v12.14.0` (Use node `v12.14.0`)

2. [Install Polymer CLI](https://polymer-library.polymer-project.org/3.0/docs/install-3-0)

`npm install -g polymer-cli`

3. Install necessary packages

`npm install`

4. Run the website

`polymer serve --npm -p 5000`

5. Open `http://localhost:5000/` in the browser

---

(From the original README)

## Configuration ##
First, create a client ID for Web applications from the [Google Play Developer
Console](https://play.google.com/apps/publish) within the project that you
want to manage.

Replace `REPLACE_CLIENT_ID` in `index.html` with your app's client ID and also replace
`REPLACE_APP_ID` in `assets/js/constants.js` with the app ID for your Games Services ID
from the Google Play Developer Console.

## Using the sample ##
When you open the sample, you will notice four tabs:

1. Achievements
2. Leaderboards
3. Events/Quests
4. Snapshots

Each of these tabs corresponds to the Play Games Services features associated
with that feature area.

### Achievements ###
From this page, you can:
* Unlock achievements
* Increment achievement counts
* Reset achievements
* Reset all achievements

This is useful for when you want to simulate the achievement features of your
game.

### Leaderboards ###
From this page you can:

* Check leaderboards
* Show high scores for leaderboards
* Show / hide players
* Submit high scores to leaderboards
* Reset player scores on leaderboards

This is both useful for testing and for managing scores for test accounts or
hiding players who are cheating.

### Events/Quests ###
From this page, you can:
* List events
* List quests
* Simulate events
* Accept quests
* Reset quests
* Reset events for quests

This is useful for testing your quests before you publish without having to
actually play through or complete the quests.

### Snapshots ###
From this page, you can
* List snapshots
* Look at snapshot data
* Alter data within snapshots

This is useful for testing your snapshot data.

**Note** Writing snapshot data from the Web API is experimental and should not
be done on production data.
