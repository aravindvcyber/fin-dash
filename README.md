# fin-dash

## Checkout the below links

Reachout to me in twitter if the below links are not working 
https://twitter.com/Aravind_V7

https://github.com/aravindvcyber/fin-dash

https://dev.d3odqnpbho0yuf.amplifyapp.com


## Architecture Diagram

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/yh8z62zqgh83wc637zft.png)

![workflow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ikm1ehwr17tpztwc16tj.gif)
## Inspiration
Fin Dash - This is a real-time dashboard that could help users with access to a host of financial data. Here with regards to this hackathon, I decided to use the Currency conversion rate to calculate the forex with the newly available NextJs SSR app hosted on amplify using data exchange services from Rearc currency exchange API.

### Video (Click to play in youtube)

[![Watch Video in youtube](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xfnvoif7uqn8l8983w1y.png)](https://youtu.be/L4gTV099XJQ)
## What it does
In this project, an amplify hosted NextJs app that could help users with various data exchange APIs like Rearc API with real-time currency exchange rates, macroeconomic rates, and other events is planned to be built. Here Amplify and NextJs SSR is strategically used to make the site simple, optimized, and secure enough to be used by anonymous users as well.

![home](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/lwz0mwjdjennjli5ubmt.png)
![exchange](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xfnvoif7uqn8l8983w1y.png)

![data exchange](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/g49phmyq5ej5lj1mmorw.png)

## How we built it
An amplify web app that could help users with various data exchange APIs from Rearc API with real-time currency exchange rates, macroeconomic rates, FDA news, and events would be built.
NextJS is used for SSG and SSR capabilities to make the site simple and optimized yet making use of server-side rendering capabilities.
Amplify backends are integrated with limited access to data access capabilities utilizing API gateway and AWS SDK client integrations using functions.
LocalStorage is also set up to reduce the number of API requests unless it is needed.
API gateway caching could also be set up to minimize resource consumption and function concurrency requirements if the environment requires it, since it is only a REST endpoint per design for the get requests, for now, it is turned off to reduce cost

![amplify studio](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/z41lypylguch0c4ij43m.png)
## Challenges we ran into
Authenticating requests to data exchange proxy is the challenge I find hard to solve, where I initially used app sync resolvers with both JS and VTL with IAM role, but the HTTP response had key-value data which I found hard to bring into Graphql schema until I use all the property names. Hence I decided to go with REST-based API gateway proxy to invoke the data exchange API securely with AWS SDK integrations for data exchange which avoids direct HTTP calls and also does not require an AWS authentication header to be created every time by adding suitable IAM policy necessary for the execution role.

Further, this is my first NextJs project, inspired to try it out after finding the release of NextJs hosting in amplify, lot of concepts to be summarized in the very last weekend before the end of submission since I only started 3 days before hackathon submission ends
## Accomplishments that we're proud of
Able to make use of the blew new features announced recently to bring this site to reality.

🚀 AWS Amplify Hosting announces Next.js 13 support!
🎉 SSR, API routes
📸 Image optimization
🏁 Faster builds
🔎 Amazon CloudWatch Logs integration

Appsync Javascript resolvers for HTTP based is tried in this project but later it was replaced with other considerations in mind to connect to the data exchange endpoint.

![next js](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/o2hpfdgrj1rljxffwlks.png)
## What we learned
In this opportunity, I have tried to use amplify NextJs SRR for secure, simple, and optimized hosting and API services are completed.
Further, I tried various means to connect data exchange services, but I wanted to make it available for anonymous users yet secure, so I decided to use NextJs SSR for optimized rendering and secure API access to data exchange API.
I have used an API gateway proxy to invoke lambda with acts as a client for Data Exchange service integration using AWS-SDK. This avoids using aws token generation for http api, since I can use the execution role policy for making client level sdk requests from lambda data exchange directly.

![data exchange api access](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4nhi7ooawfejyp6y111x.png)

## What's next for Fin Dash 
Planning to include user-level customizations with other addons in the dashboard
Dbnomics  Api, MediaWiki Api, and openFDA API are also planned. 
Maybe I may try out other free APIs if I had some time later.
