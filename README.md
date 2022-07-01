# Wikipedia Aggreagator 

Have you ever wanted a to be able to acess multiple wikipedia articles with one search term? Wiki-find can do just that. This service is intended to give the user a smorgasbord of different results by acessing the MediaWiki Action API and returning and displaying your results on a browser in the visual style of cascading cards.

It can be very useful to diplay information in this 'mind mapping' way. The benifits include;
  * It helps you remember and recall information.
  * It helps you learn new concepts.
  * It's a fun way of learning.
  * It makes complex ideas easier to understand. 
  * It improves your presenting.
  * It boosts your creativity.
  * It improves productivity.


![Responsice Mockup](https://github.com/lucyrush/readme-template/blob/master/media/love_running_mockup.png)


## Features 

In this section, you should go over the different parts of your project, and describe each in a sentence or so. You will need to explain what value each of the features provides for the user, focusing on who this website is for, what it is that they want to achieve and how your project is the best way to help them achieve these things.



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
