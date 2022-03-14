## Code and Design Specification

## Requirements

### Functional Requirements

#### Primary

- Users can search for existing discussion bibliographies
- Users can create their own discussion bibliographies
- Users can add sources to bibliographies
- Users can vote on sources in bibliographies
- Users can read sources they find in bibliographies
- Users can share their bibliographies via a link
- Sources will be clickable to redirect users to the source website
- Bibliographies have a discussion title, two “sides” with titles, and a list of numbered sources per side

#### Secondary

- Users can copy sources from other bibliographies
- Users can load multiple sources at once
- Sources will appear in MLA format
- Popup encouraging responsible voting before voting
- The users will have the option to go through a tutorial to learn how to use the website

### Technical Requirements

#### Primary

- Starting a new bibliography will send a request to the backend with bibliography title and the title of each side. A link to the bibliography will be generated and the bibliography will be displayed at that link.
- Adding a new source to a bibliography will send a request to the backend with source info and the source will be displayed on the bibliography.
- Voting on a source will send a request to the backend and the votes will be updated on the bibliography along with a way for users to know they have already voted on a source and can’t vote again.
- Searching for words will query the list of discussions on the backend for matching discussion titles and links.

#### Secondary

- Clicking the copy button next to a source will create a pop up allowing users to specify the bibliography to copy to
- There will be another + button under the currently inputted source information to create fields for another source and clicking the final create sources button will send all of those sources to the backend to be displayed
- The backend will parse the user source input to an MLA string before returning that back to the front end
- Clicking the tutorial button will initiate an animation with clickable buttons that walk the user through the website

### Usability Requirements

#### Primary

- Bibliographies are intuitive to read
- Links to sources are easy to find and click
- Searching is accurate

#### Secondary

- Site is accessible for users using screen readers

## Storyboard Flows

#### Storyboard 1: You go to the website to start a debate

#### Storyboard 2: You go to the website to glean information about a debate

## Summary:

Our UML diagram addresses all of our primary functional requirements. Starting with the landing page, we showcase our users two main capabilities: search an existing bibliography or create a new bibliography. This leads into either the search results page or the create bibliography page. Search result page would show existing bibliography pages related to the query, and creating bibliography would lead the users to a form. Clicking a search result would guide the user to the corresponding Bibliography page and filling the new page form and saving it would guide the user onto their own Bibliography page. Then the users are able to access our main features: add a new source, view a source, rate a source, and share a source. Two of the features, rate and share a source, have an additional confirmation popup component that seeks to double check that the user has read the source already. Finally, the add source feature allows users to add a new source. Technical requirements are fulfilled through the functions labeled on the arrows between pages. The page distinctions will allow us to have a clean UI to fulfill our usability requirements.
