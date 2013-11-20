OpenTable front-end task
========================

Thanks for taking the time to complete our front-end test.  We hope you find it straighforward yet interesting - it is representative of the work the front-end team is currently undertaking at OpenTable.

Please fork this repository, add your completed test and submit a pull request to send us your work.

If you have any questions along the way please feel free to email John Catterfeld (Senior Front-End Developer) at jcatterfeld@opentable.com or tweet [@jcatterfeld][tweet].

## The task

We are rebuilding our existing [Search Results][livesearchresults] and [Restaurant Profile page][liverestaurantprofile] for toptable.co.uk.  This test will focus on specific elements within each page, so the pages required and part-wireframe and part-finalised code.  

Please submit two pages, a **search results** page and a **restaurant page** based on the linked wireframes.

The pages should meet the following acceptance criteria.

### Search Page
- Page visually looks like the supplied wireframe
- When I click search, [a call is made to an API][api]
- The data returned from the API is rendered into a results table
- Clicking a restaurant name takes me through the profile page

### Profile Page
- Page loads as shown in the profile page wireframes and is populated by data from the [API][api-rid]
- When I search for the date, time and covers, [another call is made to the API][api-availability] to get back availability
- The timeslots are rendered in the booking box

#### Bonus points for
- CSS preproccesor
- JavaScript unit tests
- Use of a client-side framework

The wireframes serve as a guideline for how the page should be laid out. Feel free to impress us with a beautiful, clean design :)

[tweet]: http://www.twitter.com/jcatterfeld
[mailto]: mailto:jcatterfeld@opentable.com,bholland@opentable.com
[livesearchresults]: http://www.toptable.co.uk/s/?datetime=31/12/2013%2019:00&covers=2&metroid=72&regionids=5322&tests=EnableHistory
[liverestaurantprofile]: http://www.toptable.co.uk/roux-at-the-landau
[api]: https://raw.github.com/opentable/front-end/master/test/example-data.json
[api-rid]: https://raw.github.com/opentable/front-end/master/test/example-data.json?restaurantId=1234
[api-availability]: https://raw.github.com/opentable/front-end/master/test/example-data.json?restaurantId=1234&datetime=01/01/2014%2019:00&covers=2