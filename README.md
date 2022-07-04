# Wikipedia Aggregator 

Have you ever wanted a to be able to acess multiple wikipedia articles with one search term? Wiki-find can do just that. This service is intended to give the user a smorgasbord of different results by acessing the MediaWiki Action API and returning and displaying your results on a browser in the visual style of cascading cards.

It can be very useful to diplay information in this 'mind mapping' way. The benifits include;
  * It helps you remember and recall information.
  * It helps you learn new concepts.
  * It's a fun way of learning.
  * It makes complex ideas easier to understand. 
  * It improves your presenting.
  * It boosts your creativity.
  * It improves productivity.


## Features 

Wiki-Find is minimal in both it's approach and design. The main feature is the search input box which connects the end user to Wikipedia, a free online encyclopedia created and edited by volunteers around the world and hosted by the Wikimedia Foundation.

After you complete your search and the Wiki API returns your results you will be confronted with the applications second main feature; Data visualisation. A cascading card style display will present your search results in real time in both an organised and arranged manner. 

An animation will be actived if you hover over each article independently, making it easy to navigate multiple articles.

### Features Left to Implement

(It should be noted that a feature that lets the user save his/her history is currently being planned for a future update)

## Testing 

In this section, you need to convince the assessor that you have conducted enough testing to legitimately believe that the site works well. Essentially, in this part you will want to go over all of your project’s features and ensure that they all work as intended, with the project providing an easy and straightforward way for the users to achieve their goals.

In addition, you should mention in this section how your project looks and works on different browsers and screen sizes.

You should also mention in this section any interesting bugs or problems you discovered during your testing, even if you haven't addressed them yet.

If this section grows too long, you may want to split it off into a separate file and link to it from here.


### Validator Testing 

- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-institute-org.github.io%2Flove-running-2.0%2Findex.html)

- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Fcode-institute-org.github.io%252Flove-running-2.0%252Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css)

- Javascript
  - No errors were found when passing through the official Javascript validator [JSHint](https://jshint.com/)
### Unfixed Bugs

You will need to mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a big variable to consider, paucity of time and difficulty understanding implementation is not a valid reason to leave bugs unfixed. 


#### HTML Structure

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

#### API DOCS

- [wiki docs](https://www.mediawiki.org/wiki/API:Main_page)

- ready to go url's

#### Initial Setup

- select form, input, results
- listen for submit events
- if empty value, display error
- create fetchPages()
- pass valid input value into the fetchPages()

#### Fetch Pages

- display loading while fetching
- construct dynamic url
- display if error
- display error no items
- create renderResults()
- pass valid results into renderResults()

#### Render Results

- iterate over the list
- pull out title, snippet, pageid
- setup a card
- set results with div.articles and list inside
