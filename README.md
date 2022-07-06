# Wikipedia Aggregator 

Have you ever wanted a to be able to acess multiple wikipedia articles with one single search term? Wiki-find can do just that. This service is intended to give the user a smorgasbord of different results by acessing the MediaWiki Action API and returning and displaying your results on a browser in the visual style of cascading cards.

It can be very useful to diplay information in this 'mind mapping' way. The benifits include;
  - It helps you remember and recall information.
  - It helps you learn new concepts.
  - It's a fun way of learning.
  - It makes complex ideas easier to understand. 
  - It improves your presenting.
  - It boosts your creativity.
  - It improves productivity.


## Features 
### search input box 
Wiki-Find is minimal in both it's approach and design. The main feature is the which connects the end user to Wikipedia, a free online encyclopedia created and edited by volunteers around the world and hosted by the Wikimedia Foundation.
### Wiki API 
your results you will be generated and delivered by the applications main feature; 
[wiki docs](https://www.mediawiki.org/wiki/API:Main_page)
### Data visualisation
 A cascading card style display will present your search results in real time in both an organised and arranged manner.An animation will be actived if you hover over each article independently, making it easy to navigate multiple articles. If you click on an article the browser will automatically open the corresponding Wikipedia article in a new window.
## Existing Structure

### HTML Structure
- section.wiki
  - div.container
    - img
    - h3(text)
    - form.form
      - input.form-input type='text'
      - button.submit-btn (search) type='submit'
  - div.results
    - div.articles
      - a
        - h4
        - p (lorem20)
### Initial Setup
- select form, input, results
- listen for submit events
- if empty value, display error
- create fetchPages()
- pass valid input value into the fetchPages()
### Fetch Pages
- display loading while fetching
- construct dynamic url
- display if error
- display error no items
- create renderResults()
- pass valid results into renderResults()
### Render Results
- iterate over the list
- pull out title, snippet, pageid
- setup a card
- set results with div.articles and list inside


## Features Left to Implement

A feature that lets the user save his/her history is currently being planned for a future update. This would allow a user to recall his past search terms and acess thier respective search thereby creating a sketch books of sorts for recalling information. Javascript is also an ideal technology for this purpose making the feature easy to implement. Using local Storage to maintain some sort of user state e.g. starred articles e.t.c

## Testing 

Responsive display will automatically adjust the size and format to fit different media devices across the web. This means that your responsive display can display within a mobile app while also appearing correctly on a labtop computer or tablet device. This is achieved through the use of media queries.

All my projects features are working and have been extensivley tested at the time of publication.


## Validator Testing 


- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-institute-org.github.io%2Flove-running-2.0%2Findex.html)

- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Fcode-institute-org.github.io%252Flove-running-2.0%252Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css)

- Javascript
  - No errors were found when passing through the official Javascript validator [JSHint](https://jshint.com/)


## Deployment

- The site was deployed to GitHub pages. The steps to deploy are as follows: 
  - In the GitHub repository, navigate to the Settings tab 
  - From the source section drop-down menu, select the Master Branch
  - Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment. 

The live link can be found here - https://bariryan.github.io/p5jsCodeInstitute/

## Credits 

This inspiration for this project was largley inspired by https://github.com/john-smilga/javascript-basic-projects