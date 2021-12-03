# 1. Introductoin

**Airbnb, Inc.** is an American company that operates an online marketplace for lodging, primarily
homestays for vacation rentals, and tourism activities. It allows you to rent apartments (or even
entire houses) from people all over the world, almost everywhere in fact. The platform really
revolutionized the world of accommodations. Price is one of the main factors guests consider when
choosing where to stay, which even decides a guest's first and last impression. Also, from the
perspective of landlords, no matter how beautiful your space, if it’s priced higher than comparable
listings in the area, there’s a good chance you’ll miss out on bookings. Additionally, unfair pricing is
able to drive up the rental prices in the local areas, disturb economic order, and harm the local
economy. So the pricing strategy is a key player in the Airbnb business and even , you have to
make sure that the price defines the maximum value of the product and at the same time it must
appeal to the customers, and the whole community can benefit from it.
# 2. Data inspection
We get data from Inside Airbnb which provides data that quantifies the impact of short-term rentals
on housing and residential communities. We choose New The NYC dataset contains 37274 observations with 74 variables. 

![variables](http://m.qpic.cn/psc?/V13deus81tRRMD/45NBuzDIW489QBoVep5mccUo9Go6MyHhZbvVZy2oVjkVMiZXQketbzbB4B1.8NNVwAukP41.CeL4DAEeS4gwxWr0rpG5kXNZ70qIubJZy8w!/b&bo=OgNVAQAAAAADF18!&rf=viewer_4)

This is a complex dataset including text(space, neighbourhood,transit,etc.), time(host_since,etc.), numeric(latitude, longitude, price, etc.) and logical(host_is_super_host, host_identity_verified) variables. Ignoring some useless variables such as url and zip code, we could conclude that all variables could be divided into two scopes:
information about the house and information about the host. 

+ #### The information of the house, including
>+ **Basic information of the listing**: id, listing_url, scrape_id, last_scraped, name, description 

>+ **Description of the property**: accommodates, bathrooms, bathrooms_text, bedrooms, beds, amenities, neighbourhood_x

>+ **Host's requirements for tenants**: instant_bookable

>+ **Longitude and latitude of the listing**: latitude, longitude

>+ **Feedback rating of various aspects of the listing**:  first_review, last_review, reviews_per_month, review_scores_rating, review_scores_accuracy, review_scores_cleanliness, review_scores_checkin, review_scores_communication, review_scores_location, review_scores_value, number_of_reviews, number_of_reviews_ltm, number_of_reviews_l30d

>+ **Additional information about the listing**: minimum_nights, maximum_nights, minimum_minimum_nights, maximum_minimum_nights, minimum_maximum_nights, maximum_maximum_nights, minimum_nights_avg_ntm, maximum_nights_avg_ntm, calendar_updated, has_availability, availability_30, availability_60, availability_90, availability_365, calendar_last_scraped

+ #### The information about host, including 

>+  **Airbnb's unique identifier for the host/user**: host_id

>+ **The basic information of the host**: host_url, host_name, host_since, host_location, host_about, host_is_superhost, host_total_listings_count, host_listings_count, host_thumbnail_url, host_picture_url, host_neighbourhood, license

>+ **Landlord's online quality**: host_response_time, host_response_rate, host_acceptance_rate, 

>+ **Requirement of the host**: host_verifications, host_has_profile_pic, host_identity_verified

>+ **Information of the listing number**: calculated_host_listings_count, calculated_host_listings_count_entire_homes, calculated_host_listings_count_private_rooms, calculated_host_listings_count_shared_rooms

And we will use this dataset to build our
model and provide valuable insights for Airbnb, hosts and tenants.
