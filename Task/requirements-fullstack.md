# Test Specifications and Requirements

## Abstract

You should develop a simple website with front-end and back-end logic. The back-end provisions data for a table which is shown on the front-end part (a single web page). The table should show only a portion of data and use pagination to browse through entire dataset. It also should allow to sort data by columns (asc/desc).

## Requirements

### Functional Requirements

1. Implement navigation menu (top left coner):
   - mouse hover on any item should make it opaque
   - mouse hover on a main menu item should open its sub-items
2. Implement selectable language flags (top right coner):
   - mouse hover should make a flag opaque
   - select flag should be opaque
3. Implement toggle boxes (the right panel):
   - only one box should be opened at a time
   - click on a box to open or close it 
4. Implement a data table:
   - data should be browsed by pages (100 lines per page)
   - the pagination should be present on top and bottom of the table
   - it should be possible to sort the data on a page ASC/DESC (click column's header to sort it)

### Non-Functional Requirements

1. Front-end requirements:
   - Page UI based on Liquid layout
      - max content wrapper width: 1280px, min width: 800px
      - content centered on the page
      - right column width: 30% of content wrapper
      - left column and right column padding 10px (either column can lead the height of the page)
      - embed font for page main title (HelveticaInserat LT)
      - font sizes and box sizes may be in %, px or em
      - logo element must be fixed at all time at the left border of the page
    - Don't use ready JS (or 3rd party libraries) to implement navigation menu
    - Your script must be able to handle number of columns dynamically (i.e. more or less columns)
    - Decide on the table HTML structure by yourself (table/div... etc.)
2.  Back-end requirements:
    - Get the sample data from here: https://app.bti-sports.io/tests/FA71E469-A68C-48A5-BD00-527CCD6365A9/data.json
    - Implement a RESTful API which provisions data
    - Implement a persistence storage which is used by the API (API should not load data from the weblink above)

### Technical Requirements

1. Front-end requirements:
   - Use only Vanilla Javascript (no jQuery or other frameworks)
   - Use any styles pre-processor (SASS or LESS)
   - Use AJAX
   - Cross-browser support should be in-place (IE 11+, Edge, FF, Chrome)
2. Back-end requirements:
   - .NET Core vs .NET Framework
   - Use LINQ
   - Use asyn/await

## Tests Verification

1. Functional testing:
   - your solution should work without additional configuration (if it's required, you need to accompony your solution with notes where you explain all required configuration)
   - the web site behaves as expected as per the requirements
2. Non-Functional testing::
   - the code structure, its quality and reusability
   - the adhering known programming principles and best practicies

### Bonus points  

Bonus points to the task completion are going to be awarded for:
- TypeScript 3.x
- React 16.6.x (NO REDUX!)
- Unit Tests
- Code Linting
- Swagger

### Recommendations

- Remove all unnecessary stuff from the solution source code, your source code must keep only required files, classes and logic