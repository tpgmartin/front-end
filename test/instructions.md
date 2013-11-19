OpenTable front-end task
========================

Thank you for taking the time to complete our front-end test.  We hope you find it straighforward yet interesting - it is representative of the work the front-end team is currently undertaking at OpenTable.

Please fork this repository, add your completed test and submit a pull request to submit your work.

If you have any questions along the way please feel free to contact John Catterfeld (Senior Front-End Developer) at jcatterfeld@opentable.com or tweet [@jcatterfeld][tweet].

## The task

Below is some acceptance criteria for each page:

### Search Page
- Page loads as shown in the search page wireframe
- When I clicks search, a call is made to an [API][api]
- The data returned from the API is rendered into a results table
- Clicking a restaurant name takes me through the profile page

### Profile Page
- Page loads as shown in the profile page wireframes and is populated by data from the API [API][api-rid]
- When I search for the date, time and covers, another call is made to the API [api-availability] to get back availability
- The timeslots are rendered in the booking box

#### Bonus points for
- CSS preproccesor
- JavaScript unit tests
- Use of a client-side framework

The wireframes serve as a guideline for how the page should be laid out. Feel free to impress us with a beautiful, clean design :)

If you have any questions then don't hesitate to [email me][mailto]

[tweet]: http://www.twitter.com/jcatterfeld
[mailto]: mailto:jcatterfeld@opentable.com,bholland@opentable.com
[api]: http://labs.benholland.me/api/data.json
[api-rid]: http://labs.benholland.me/api/data.json?restaurantId=1234
[api-availability]: http://labs.benholland.me/api/data.json?restaurantId=1234&datetime=01/01/2014%2019:00&covers=2