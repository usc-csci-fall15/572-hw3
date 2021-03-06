# 572-hw3-CSCI572
A web-app for displaying indexed weapons data from Solr

##Youtube Video

[Team 36 CSCI 572 Weapons Visualization Video](https://youtu.be/uUo1dmmDx_g)

[![Alt text for your video](http://img.youtube.com/vi/uUo1dmmDx_g/0.jpg)](http://www.youtube.com/watch?v=uUo1dmmDx_g)


##Installation
1. To run this webapp please place the `charts` folder in the `$SOLR/solr/example/solr-webapp/webapp`.  Where $SOLR is the lucene-solr installation is located.

2. To run this open the browser and navigate to http://<SOLR_URL>:<SOLR_PORT>/solr/charts/index.html

	- e.g. http://localhost:8983/solr/charts/index.html

We have included our SOLR index in a folder named `collection2`.
To run this app with data please place the collection2 data within `$SOLR/solr/` directory.  The folder should be named `collection2`.  

##Dependencies

We leverage these dependencies

- jQuery 
- Banana
- Facetview

##Structure

The webapp sits within the `charts` folder.  The app is split into three tabs. Each tab correlates to an html page.

- D3 `-> index.html`
- Banana `-> 572-banana.html`
- Facetview `-> 572-facetview.html`

Within D3 we have 6 visualizations, and each of those visualizations rests in an iframe that we can toggle with navigation panes.

We have included banana as a tab, and we've placed the app within it's own enclosing folder.  Furthermore, We reference banana as an iframe in `572-banana.html`.

Lastly, we have included facetview as an iframe as well. This methodology is identical to what we've done for banana.




