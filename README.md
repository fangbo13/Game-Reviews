
# Game Reviews

Build a community website to review games (you can choose what type). All the game details and reviews must be stored in a database.

---

## Testing

The system should include the data for at least 5 valid games and each game must contain at least 3 sensible reviews posted from from valid user accounts (see below).

You are required to create the following accounts to allow the system to be tested. All accounts should have the password `p455w0rd`:

1. `user1`
2. `user2`
3. `user3`

---

## Feature 1

The homepage should be viewable without being logged in. After logging in the user should see an **Add game** button. Clicking this takes them to a screen where they can add a game to be reviewed. This should request the following information:

1. The name of the game.
2. The publisher.
3. A slider allowing the user to specify the year of release. The slider should start at 1980 and stop at the current year.
3. A multiline textbox where they can enter a description of the game. This should support _markdown_ formatting.
4. An image picker where the user can upload an image file showing the game box cover from their local device.

When the game is added, the following data should be automatically added to the database without requiring it to be entered by the user:

1. The username of the person adding the game.
2. The date and time of when the game was added.

> To demonstrate this feature and to prove that the form works correctly you will need to show that the data is being persisted correctly, either by running a database query or an API call depending on the platform and technology you are using.

## Feature 2

The homepage should display all the games that have been added. For each there should be the following:

1. The name of the game.
2. The year of release.
3. A thumbnail of the game box cover.

## Feature 3

There should be a **Details** button or link next to each game. This should be visible whether the user is logged in or not and should take them to a _Game Details_ page that contains all the information held on the game. Specifically it should show:

1. The name of the game.
2. The publisher.
3. The year of release.
4. The description with the markdown formatting converted to html.
5. The date (but not the time) the game was added to the site.
6. The username of the person who added the game.

## Feature 4

This feature requires you to make changes to the functionality:

There should be a review section at the bottom of the _Game Details_ page. This should only be shown if the user is logged in. It should request the following from the user:

1. A slider to allow the user to rate the game out of 5.
2. A multiline text box where the user can add their review. This should support _markdown_ formatting.

In addition to this data, the system should store:

1. The username of the person leaving the review.
2. The date and time when the review was posted.

If there have been any reviews added for a game, these should appear on the _Game Details_ page between the game description and the review section. Each review should include the following:

1. The rating awarded shown out of 5.
2. The username of the person who wrote the review.
3. The date the review was posted (but not the time).
3. The review text with the _markdown_ converted to html.

