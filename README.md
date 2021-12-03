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
## data inspection
We get data from Inside Airbnb which provides data that quantifies the impact of short-term rentals
on housing and residential communities. We choose New The NYC dataset contains 37274 observations with 74 variables. 




![variables](http://m.qpic.cn/psc?/V13deus81tRRMD/45NBuzDIW489QBoVep5mcYYCpg8M.OCMxX4iLowMhOPgWwBe8hYBEobq2uByMc0Mx2tCyl.*1PrR8GiaeF7n4RelJfP0ms26822YYXmeSFc!/b&bo=TwTHAQAAAAADJ48!&rf=viewer_4)


This is a complex dataset including text(space, neighbourhood,transit,etc.), time(host_since,etc.), numeric(latitude, longitude, price, etc.) and logical(host_is_super_host, host_identity_verified) variables. Ignoring some useless variables such as url and zip code, we could conclude that all variables could be divided into two scopes:
information about the house and information about the host. And we will use this dataset to build our
model and provide valuable insights for Airbnb, hosts and tenants.
