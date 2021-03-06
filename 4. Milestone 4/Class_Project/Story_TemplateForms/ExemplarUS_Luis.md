# As a user I want to be able to search and find peaks/mountains by name and display their expeditions with 
  relevant expedition information so users, agencies, and visitors to our site can find relevant information. For users, this will help
  them stay informed about their next expedition based on a certain peak. Moreover, it can be useful 
  information for agencies in their decision making process and for any reason they may have.

## ID: #176694122
## Effort Points: 2
## Owner: Luis Olvera
## Feature branch name: Peaks_Expeditions

## Assumptions/Preconditions
  Originally I had thought it was going to be a lot easier but then I realized that there was a lot more 
  work involved. Especially since their is no queried data for an expeditions 'name' in our database, I 
  had to use Peak's ID to display all expeditions that matched a specific Peak's ID. This way, the user can
  search a mountain/peak by name, click on the name, and then be prompted to a new page with all the 
  expeditions relevant to that specific peak.

## Description

1. The user is able to search a mountain/peak by name.
2. Mountains are displayed by beginning keywords of what the user searched.
3. Users can click on the mountains displayed, to be redirected to a different page
4. Upon being redirected, users are able to see all the expeditions for that current mountain/peak
5. All expeditions for specific peak, are rendered onto the page, and all of the expedition's information

Include links to modeling diagrams or anything else referenced or needed to complete this story.

## Acceptance Criteria
[Try to write criteria that, when true or satisfied mean that it is correct and you're done. Write them in the "If ___ then ____" format, 
for if you do this then you should expect this result, for defining the correct behavior that shows the feature works as requested]

1. If a user searches a peak/mountain by its full name or similar keywords then the mountain will 
    apear below the search bar when the user clicks on the search button.
2. If a user clicks on a peak/mountain when they are displayed below the search bar then it will 
    redirect them to a new page with all expeditions relevant to that peak/mountain.
3. If a user clicks on 'Home Expeditions' on the nav-bar then it will redirect them back to the 
    main home page.
4. If a user clicks on 'Searh_Peaks' on the nav-bar then it will redirect them to page where they
    are able to search for peaks/mountains.

## Tasks
1. Make sure peaks/mountains can be searched.
2. Make sure that peaks/mountains can be displayed based off of what was searched
3. Make sure that user can then click and then view all expeditions from a specific peak/mountain
4. Make sure the user can view all relevant information on the expeditions based on the peak/mountain

## Dependencies
Other user stories that this one depends on

## Any notes written while implementing this story
1. In order to pass back all the expeditions on a specific peak, then I have to pass back the ID and
    filter out all the expeditions that only match that specific peak.