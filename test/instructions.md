OpenTable Front-End Task
========================

Greetings potential OpenTable ~~worker drone~~ employee. The following task is designed to allow us to assess a candidate's ability to produce the standard of work we're looking for, but also give them the freedom to impress us.

Once you've finished the task, zip it up and send it to jcatterfeld@opentable.com.

## The Task

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

[mailto]: mailto:jcatterfeld@opentable.com,bholland@opentable.com
[api]: http://labs.benholland.me/api/data.json
[api-rid]: http://labs.benholland.me/api/data.json?restaurantId=1234
[api-availability]: http://labs.benholland.me/api/data.json?restaurantId=1234&datetime=01/01/2014%2019:00&covers=2