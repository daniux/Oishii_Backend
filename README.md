# Oishii_Backend
This is the backend directory of Oishii project. For details regarding this project, please refer README.

Oishii is a restaurant search and recommendation APP + service to improve personal experience for foodies. 
This backend includes a database and a java service to process data. 
I guess many of you will ask why do we need this? We have Yelp already
So the difference with Yelp: Oishii APP can provide personalization recommendation feature.

Here is the basic structure of these codes:

// Recommendation based on GEO distance and similar categories.
package algorithm:
	GeoRecommendation.java

// Database connection with MYSQL db.

package db:
	MySQLConnection.java
	MySQLDBUtil.java
	MySQLTableCreation.java
	
// Detail instance definition of item (restaurant here).

package entity:
	Item.java

// Connection with external API.

package external;
	YelpAPI.java
	
// Remote Procedure Call for different Servlets.

package rpc:
	ItemHistory.java
	Recommendation.java
	RpcHelper.java
	SearchItem.java
	

Implementaion Level:
	API
	Show items near your location
	Set favorite items
	Recommend new items
