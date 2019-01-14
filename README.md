# theScore iOS Interview
At theScore, we're always looking for intelligent and resourceful iOS developers to join our team. To help us evaluate new talent, we have created this take-home interview assignment. This assignment should take you no more than a couple of hours.

**All candidates must complete this before the possibility of an in-person interview. During the in-person interview, your submitted project will be used as the base for questions.**

### Why a take-home interview?
In-person coding interviews can be stressful and can hide some people's full potential. A take-home gives you a chance work in a less stressful environment and showcase your talent.

We want you to be at your best and most comfortable.

### Understanding the problem
In this repo are the files [`leagues.json`](leagues.json) and [`leagues/{league_slug}.json`](leagues/nhl.json).
The leagues file contains a list of leagues. Each entry contains the following information
* `full_name`: League's full name (NHL Hockey, NFL Football, ...)
* `slug`: League's slug (NHL, NBA, ...)

```json
[
  {
    "full_name": "NHL Hockey",
    "slug": "nhl",
  },
  ...
]
```

The leagues details file contains the list of teams playing in that league. Each entry contains the following information
* `full_name`: The team's full name (Boston Bruins)
* `name`: The team's name (Bruins)
* `location`: The team's location (Boston)
* `logo`: The URL to the logo of the team
* `colour_1` and `colour_2`: The team's colours

```json
[
  {
    "location" : "Boston",
    "full_name" : "Boston Bruins",
    "logo" : "https://d12smlnp5321d2.cloudfront.net/hockey/team/1/logo.png",
    "colour_2" : "343434",
    "name" : "Bruins",
    "colour_1" : "FDB930"
  },
  ...
]
```

### Requirements
Your task is to create an iOS application that has two screens; a League list, and a Team list.

* The League List screen
    * Displays all of the leagues contained within [`leagues.json`](/leagues.json) in alphabetical order (based on the `full_name`)
    * Only full names should be displayed for each league.
    * When the user taps a league it should launch the league's teams list page
    * **Bonus:** Allow the user to search the list by slug or full name.
* The Team List screen
    * Displays the list of teams playing in a specific league selected from the League List
    * The team logos and full names must be displayed. The logo must be positioned on the left side and the name must be right next to it. When the team has no logo, the team's primary colour will be displayed instead. If both information are not present, the spacing used for the image should be removed.
    * **Bonus:** Allow the user to search the list by name, location or full name.
* Add tests wherever you see fit.
* Please consider the provided JSON files as if they were a REST API.

### Submitting a solution
1. Download this repo
2. Complete the problem outlined in the **Requirements** section
3. In your personal public GitHub repo, create a new public repo with this implementation
4. Provide this link to your contact at theScore

We will evaluate you on your ability to solve the problem defined in the requirements section as well as your choice of design patterns, libraries, unit tests, and general coding style.

### Help
If you have any questions regarding requirements, do not hesitate to email your contact at theScore for clarification.