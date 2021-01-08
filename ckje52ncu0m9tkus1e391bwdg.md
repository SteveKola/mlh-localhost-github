## Overview: Building an Apartment Rent Pricing App

***An end-to-end machine learning application development process walkthrough.***

![house_rent.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1610092492453/GFaXgy0tC.jpeg)

Hey folks, season greetings to y'all! 

I finally decided to work more on building end to end machine learning applications so I'm currently working on an apartment rent pricing app, which you'd use if you are (hypothetically)looking for an apartment in any of the megacities in Nigeria - think Lagos, Abuja, Port Harcourt, Ibadan, etc. I haven't decided on a cool name for the app yet. I'm thinking of ApartRent or something. The name would probably sort itself out, I'd worry more about the development, for now.

If you have ever had to search for an apartment before, you'd appreciate how frustrating the process is. I did, when I got into college. I didn't want to stay in the school hostels, and it was horrible traversing the whole neighborhood trying to find the right apartment at the right price and best opportunity cost.

Most times, you'd have a target spot you'd want the apartment to be located at, and a specific amount of money that you're willing to cough up. Also, there are few trade-offs you'd have to compromise on; For instance, would you take a serviced apartment over one that is closer to the park or bus stop? How much are the different perks worth, compared to each other? How about we employ Machine Learning to take care of decisions like this for us?

So in this series, I'll walk you through the whole development process, from start to finish. The steps will include;

- **Data Gathering via Web Scraping** - we'll scrape apartments listing data from http://propertypro.ng/, the no 1 real estate listing website in Nigeria.
- **Data Wrangling** - Cleaning the data and preprocessing into an acceptable format we could work with. This should take about 50% to 60% of our development time.
- **Feature Engineering** - A model is only as good as its data. We will create new features out of the existing columns. We'll also use Google Maps API to generate some key geo features.
- **Modeling and Model Deployment ** - We'll fit the ready data into a model algorithm, so we'd be able to make predictions on new data. Then we'll productionize the model (90% of Data Science projects don't make it to production, so we'd be pretty proud of ourselves at this point) by converting it to a SavedModel file and deploy in a web app/framework. We'll be using Streamlit or Flask. I'm indecisive yet.
- **Web App Deployment on a Serverless Cloud Provider** - So other folks could make use of our finished ML-powered web app from wherever they are.

So folks, let's get started! 

![let'sdothis.gif.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1609497065037/EvUzNoND5.gif)

I will regularly update this article with the links to the tutorial articles as I publish them. Have fun!

And yeah… Say hi to me on  [Twitter](https://twitter.com/steveddev)  and connect with me on  [LinkedIn](https://www.linkedin.com/in/steven-kolawole-80/) .