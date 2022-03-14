# Digital Prototype

## Recap: The Problem and our Research

Online anonymity and rapid sharing allows misinformation to disseminate quickly and with little consequence
to the people sharing it. Moreover, there are many different types of misinformation, including but not limited to:
incomplete or biased information, and improper statistical figures.

Through our user study (consisting of participants mostly in their early 20s and in higher education)
we were able to find that our users care about getting easy and efficient access to information,
trust well-known publications, and the majority only tend to lurk on online platforms.
Thus, our project Greatest Online Anti-misinformation Tables (GOAT) seeks to encourage users
within online and offline discussion to be cautious about misinformation.
Our platform encourages participants to utilize reliable sources and debate the validity of said sources.

[Check out our work!](https://github.com/UWSocialComputing/Wild-Swaying-Goats-Project)

![Final Bibliography Page](/Wild-Swaying-Goats/data/pictures/finalBibPage.png)

## Our Design Choices

In our final prototype some design choices we made after our initial prototype feedback was following
a neutral color scheme of gray and blue. We wanted to ensure that color was not an external factor
that swayed the audience when reviewing a source. Another feedback we received was on the voting slider.
We incorporated an initial average score indicator and a vote button for the user to rate the source.
Once the user has submitted their vote, the voting slider and vote button will turn gray.
We have this component for each source as we are not expecting users to be able to sift through all the sources.
Lastly, the add-new-source button lives at the bottom to contain a bit of friction for the user.
Our intention is that the user is forced to at least skim over existing sources before adding their own.

![Landing Page](/Wild-Swaying-Goats/data/pictures/finalLandingPage.png)

![Bibliography Page Voting Slider](/Wild-Swaying-Goats/data/pictures/finalVoting.png)

## Our Technical Choices

Our final prototype is a React web app. It has 4 types of pages: the landing page with links to all bibliographies,
a page to add new bibliographies, individual bibliography pages, and a page to add new sources to the individual bibliography pages.
While we don’t have a backend, we have preloaded state stored on the frontend that is responsive to user input.
Adding bibliographies, adding sources, and voting on sources will change the state of the app until the page is refreshed.
We built our React components using the MUI component library.

![Add Bibliography](/Wild-Swaying-Goats/data/pictures/finalAddBibPage.png)

![Add Source](/Wild-Swaying-Goats/data/pictures/finalAddSourcePage.png)

## Roadblocks faced

Due to our limited time constraint, we decided to forego our Firebase back-end database in favor of a JSON blob “database”.
This helped us focus more on creating functionalities without having to create code to communicate with Firebase.
However, because of this, some functionalities faced some bugs, such as in adding bibliography pages.
We had to create a global state that could be accessed as props by all of our components as each component could not contact a database to fetch data.
One roadblock we ran into was adding new react-router-dom <Route> components as the user added bibliographies to the app.
We found a workaround that allowed us to render one new bibliography page, but did not find a way to add multiple.
So, our app is currently only able to display one new bibliography page.