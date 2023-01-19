### Chalhoub Assignment

#### Case Study - Magento 2.4 - Shopfinder GraphQL

As a new joiner of our super secret laboratory is requested to you create the most exciting Shopfinder API ever seen on the 7 galaxies. The
design, the shape, the velocity, and the glory are all in your hands to decide.
For the most required and desired functionality, the business wants to have a Magento 2.4 (community edition) Docker instance and a
"Shopfinder" module (described in #case2).
All required information on how to run and configure the project should be included in a readme, ideally, a non-technical person should be
able to run it.
Technical and business requirements.
#1 Magento docker instance
The project should include a docker image that has nginx, php7 (and required modules), mysql, and magento2 in it.
We should be able to run docker-compose to spin up the project. This should build up all servers and open expose port 80, install
Magento from composer if not installed. After that, we should be able to access http://magento2.local after adding this magento2.local
to our hosts file.
Mysql should be persistent, if we shut down docker, once running it again all the saved data must still be there.
#2 Shopfinder module
We want you to prepare a module for us which can be installable with composer.
We should be able to see "Shopfinder" menu on the Content section as Imgur When we click on Shopfinder link it should list all added
shops. And it should also have filtering options as Imgur
We should be able to add/edit new shops as Imgur in screenshots we have lots of fields.
For this scenario, you just need to cover these fields
Shop name - the name of the shop, string
Identifier - a unique identifier of a shop, string
country - which should be populated by a list of countries in Magento
image - user should be able to upload an image
(Optional) longitude/latitude, string
#2 GraphQL API
The Shopfinder Module should expose a GraphQL API.
We should be able to use any graphql playground.
We should be able to use a query to fetch all the shops.
We should be able to use a mutation to update any store information.
We should not be able to delete stores from the API - Provide a proper error handling for this case.
We should be able to use a query to fetch information about a single shop based on the identifier.
(Optional) We should be able to fetch the stores near me, based on my current location.
**As a plus, consider providing unit/functional tests. If so, describe the steps to run the tests