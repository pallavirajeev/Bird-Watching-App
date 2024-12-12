# Project: Bird Watching App by Trinity Wu & Pallavi Rajeev

Welcome to our Bird Watching App! Read more to learn how to navigate this app and all the various features included for our users.

The app is organized around the following main pages: 

- Index page.  Welcomes users and shows a map of bird densities. 
- Checklist page.  Enables users to enter a checklist. 
- Stats page.  Enables users to see stats and compilations about their own data. 

## Index page

When users log in they are welcomend with an information message, describing the app briefly. Users should then see a map with a density indication of where birds have been seen. Users can view a dropdown of all the species contributing to the density heatmaps. The page also contains links to submit a checklist, view their checklists, and a “My birding” stats page. 

### Map Implementation 

Map implemented with the [Leaflet](https://leafletjs.com/) library.
 

## Checklist page

This page allows users can enter a checklist.  This page is accessed by selecting a position on the map page and clicking on the "Enter Checklist" button. Note, users will need to be logged in to enter a checklist

The checklist page has a search bar that enables species selection followed by a button to increment of decrement the number of birds seen. This information gets autofilled into a table with a pre-saved longitude and latitude from the user's map position. Users can then finish inputing their bird watching statistics including the date observed and duration observed. 

When the user is done, they can click on a "submit" button, and the checklist is saved.

Users can then return to the home page and select the "My Checklists" button to view all saved checklists. 

## User statistics

This page allows users to access the statistics of their bird watching journey. This includes:

- A list of all species users have seen, searchable
- A visualization of when users saw each species and where with corresponding map pins 
- A chart visualization of how a user's bird-watching has trended in time 

### Sample data

The databases are primed with [this data](https://drive.google.com/drive/folders/1NV5vMn0h3O5peppvBHqcdJAudPQe_Qkg?usp=sharing). 
This includes: 
- `species.csv` contains the species of birds (about 400). 
- `checklists.csv` contains the checklists.  Each checklist has a user, a location, and a data, among other fields. 
- `sightings.csv` contains the sightings.  Each sighting has a checklist, a species, and a number of birds seen.

The data comes from 10 days of eBird checklists in the area which has been modified. 

### How to Run Our App

In order to run our app, follow these quick and easy steps:

- Run 'py4web run apps' in the terminal 
- The app will be available at http://127.0.0.1:8000/birds where you will be prompted to login
- Finally, sign up or login and enjoy bird watching!