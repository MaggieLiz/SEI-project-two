Bookcation

Overview

Bookcation is a play on the idea that books can take you places. You can select a book from the library we curate and find out the current weather of the book's setting. I worked with a partner, [Jessica Strawford](https://github.com/jessicastrawford), to build this application.

![](https://lh5.googleusercontent.com/wtgPK9EzsHP1o3EbI7P0ZmXwHwnqclZSsN0r1dJXjMBxvPKToToZZ_IcgziXd-0XCrLm2e0qlU29KsI9IHtpS6M1rcfuBVDi_GL6IUXt8mcQHXjqvCRutlB2Gypy5stLMRT8qDsB=s0)

 ![](https://lh6.googleusercontent.com/pVojOMXBbGACT1qR2MVBU8ywiT37gf6H9fukQoYOc9h-uhPSJebVfJFdgfS0gnhNGO4NmHfwrqWqS96kDqfIMv-JdXAVK55dxLkpxkhZ2vnYL4F4CIVUIIH0TuEMls0vYhTYmmo_=s0)

Deployment

This web app has been deployed with Netlify and is available [here](https://bookcation.netlify.app/).

Brief

We had to use React JS to build a web app that consumes a public API. We had two days to complete this task. In addition to consuming a public API, our app also needed to have several components and be deployed online.

Technologies Used

-   HTML5

-   Sass

-   ReactJS

-   JSX

-   GitHub

Process

Jessica and I went through many iterations of the idea we wanted before landing on this final format. Originally we hoped to build an app where a user could select the weather of the place they would like to go and we would return book suggestions with that setting. For example, if you wanted to get bundled up, you would select cold weather and the app might suggest "Into the Wild" by Jon Krakauer because it's set in Alaska. This is when we began to learn the limits of external APIs.

After spending a fair bit of planning time checking what information different weather APIs could provide we settled on asking for weather for specific cities instead of asking for specific types of weather. Once the concept was finalized, we built a wireframe and began coding.

We curated our own "library" by listing books that had distinct settings. We used that dataset to create a Books Index page. Each Book Show page would then make a request to the API [goweather.herokuapp.com ](https://goweather.herokuapp.com/weather/austin)for the setting's current weather.

Once the functionality was in place we styled the app.

Challenges

Learning to work with an API for our needs was interesting. It taught me to be flexible regarding my plans for the app.

Additionally, the API seemed to change how cities were listed from time to time. So we might successfully make our request for "Bogata, Colombia" to get the weather and then the next day have to request only "Bogata." 

We also ran into an infinite loop issue when we tried to useState on our Book Show page. We needed to have the book set in state in order to use its location for the API request. We ended up using a Lazy Initial State to overcome the infinite loop.![](https://lh4.googleusercontent.com/J_Oo9wP_pbs2MaoDDjigERE82c4gMhbsSZ47w4UOYWoDxhuqdARo4BwC-qYkAC-reeIjFT_IX7F3_6DZbZ6pNuUR5852jxKhmLFVeqOZ3RfichdwKRmW89-1LCuYKmi0Wk8qq7pq=s0)

Wins

I was pleased to have a complete project to present at the end of our 48-hour timeframe.

Known Bugs

I had to hard-code the emoji weather symbols depending on the innerHTML of the city.description. Because I couldn't find a list of all the possible weather descriptions, I had to build it off the descriptions I could see. So, the list is incomplete. The page compiles as expected, it simply doesn't include the emoji.

![](https://lh6.googleusercontent.com/2o7hN5QYDTtEZi3s-2T3Nt0R0zs3u3kFutJUfZWYVvdrmEjoL_D4QlbOHvq2nWdaKFf2gQ8gVyZPjhMY3JdeeIuql_4vPIFMqaUemQnZIiHs1OpCWnXinMM28r-MevKPBkMiOh_y=s0)

Future Improvements

-   This app could be more valuable with a larger library. 

-   I would add weather 7-day forecasts to the pages. 

-   I would like to use more destination based APIs to the app to provide information like signature food items and languages spoken.

Key Learnings

This project was a useful first step in learning about APIs and using React. It was also a good lesson in working with another person toward a common objective. I was able to lean into my strengths and lean on my partner's strengths to achieve our goals.