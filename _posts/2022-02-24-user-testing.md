# User Testing

## A: Description of Medium-Fidelity Prototype

The first functionality we implemented is displaying sources that are linked to external sites. The code for it is at wild-swaying-goats-app/src/BibliographyPage.js. Components on the page are in the wild-swaying-goats-app/src/components folder. The data displayed on the bibliography page is saved in wild-swaying-goats-app/data/sources.json.

The second functionality is having a separate page to add sources to the bibliography page. The code for it is at wild-swaying-goats-app/src/AddSourcePage.js.

The user is also able to go between the two pages mentioned by clicking “Add New Source” on the Bibliography page and then selecting either “Cancel” or “Save” on the Add Source page to go back. 

Currently we have dummy data for the citation list to simulate pre-existing citations within a discussion, which we got from another [online platform](https://www.kialo.com/the-size-age-and-properties-of-the-observable-universe-allow-for-an-extremely-high-number-of-planets-on-which-life-could-1258.1680?path=1258.0~1258.1_1258.1680). We provided users with plenty of context around the purpose of our app and what would change on the page if they performed certain actions. For example, if they slid the slider to a new value, we verbally explained that the average would shift to reflect the new slider input.

## B: Screenshots of the Prototype

### Bibliography Page Components
![Bibliography Page Components](/Wild-Swaying-Goats/data/pictures/g6-bib-components.png)

### Add Source Page Component
![Add Source Page Component](/Wild-Swaying-Goats/data/pictures/g6-add-source-component.png)

## C: Findings

We learned we should display more information about sources and ratings within our bibliography tables. One idea is to show a tag of “source type,” like Wikipedia or blog or news or scientific paper. Our ratings should explicitly explain that the number displayed by the slider is the average rating from other users. 

The functionalities we implemented were basic aspects of our app, so they are somewhat cemented as features of our later prototypes. Something more variable was our slider system. We have always been curious about the best way to “rate” sources. We got enough positive feedback on our sliders that we will likely continue using them in future prototypes. Changes we will make to them, though, is to find a better way to explicitly show users the effects of their actions related to the slider. Maybe it’ll look like a submit button or the page refreshing to display changes in the average rating.

The next functionality that we’re planning to implement are a button to submit the quality rating and an average quality rating that changes with the data. After that we’re going to implement adding a source to the json file so that the Bibliography page updates after users input a source on the Add source page. Finally, a user testing suggestion that stood out to us was having small descriptions or tags of the types of sources under each source on the Bibliography page, so we might try to implement that next. In addition, we have some general css styling plans to make everything look less one dimensional, a bit cleaner, and overall more intuitive for users.
