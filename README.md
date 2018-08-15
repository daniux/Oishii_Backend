# Oishii_Backend
This is the backend directory of Oishii project. For details regarding this project, please refer README.<br/>
Oishii is a restaurant search and recommendation APP + service to improve personal experience for foodies.<br/>
This backend includes a database and a java service to process data.<br/>
I guess many of you will ask why do we need this? We have Yelp already.<br/>
So the difference with Yelp: Oishii APP can provide personalization recommendation feature.<br/>
<br/>
Here is the basic structure of these codes:<br/>
// Recommendation based on GEO distance and similar categories.  <br/>
package algorithm:<br/>
	GeoRecommendation.java<br/>
<br/>
// Database connection with MYSQL db.<br/>
package db:<br/>
	MySQLConnection.java<br/>
	MySQLDBUtil.java<br/>
	MySQLTableCreation.java<br/>  
<br/>
// Detail instance definition of item (restaurant here).<br/>
package entity:<br/>
	Item.java<br/>
<br/>
// Connection with external API.<br/>
<br/>
package external;<br/>
	YelpAPI.java<br/>
<br/>
// Remote Procedure Call for different Servlets.<br/>
package rpc:<br/>
	ItemHistory.java<br/>
	Recommendation.java<br/>
	RpcHelper.java<br/>
	SearchItem.java<br/>
<br/>
Implementaion Level:<br/>
	API<br/>
	Show items near your location<br/>
	Set favorite items<br/>
	Recommend new items<br/>
