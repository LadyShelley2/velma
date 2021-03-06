## A responsive multipurpose Ghost Theme

#### Encourage Us By Starring or Forking the repository

#### [DEMO](http://velma-redhivesoftware.rhcloud.com)

### Documentation

####How to open the admin panel
 Go to yourblogaddress/admin, so if your blog is http://example.com then you need to open http://example.com/admin

####How to install the theme in the server.

1.Go to the ghost folder then content -> themes and copy the velma theme folder in the theme folder.
2.Restart the ghost server.

####How to configure the theme  
1.Go to the admin panel and click on code injection in left side.  
2.Go to the  blog header section and copy the below code

        <script>
        	velma.url={
        //		facebook:"https://www.facebook.com/RedHive-Software-623049087845699/",
        //		twitter:"https://www.twitter.com/redhivesoftware",
        //		tumblr:"https://www.tumblr.com/blog/redhivesoftware",
        //		gplus:"http://plus.google.com/u/0/115145342026041498272",
        //		youtube:"your youtube url",
        //		linkedin:"your linkedin url",  
        //		instagram:"https://www.instagram.com/velmaredhivesoftware",  
        //		flickr:"https://www.flickr.com/photos/redhivesoftware/",  
        		end:true
        	}
        	velma.follow={
        //		facebook:'disabled',
        //		twitter:'disabled',
        //		gplus:'disabled',
        //		linkedin:{
        //			id:123
        //		},
        //		youtube:{
        //			channel:'Sic7VK9KUtKMgaWa5Nz71Q'
        //		},
        //		tumblr:{
        //			blogname:'redhivesoftware'
        //		},
        		end:true
        	}
        	velma.comment={
        //		disqus:'velma123',
        //  	facebook:'enabled',
        		end:true
        	}
        	velma.feed={
        //		facebook:'disabled',
        //		twitter:{
        //			id:'696094298215940096'
        //		},
        //		instagram:{
        //			userId:'2899013383',
        //			accessToken:'2899013383.a525e19.a119b4854c944131bbe5f6632ef76a48'
        //		},
        //		flickr:{
        //			qstrings:{
        //				id:'139052977@N02'
        //			}
        //		},
        		end:true
        	}
        	velma.newsletter={
        //		popup:true,
        //		hide:true,
        //		time:10,
        		end:true
        	}
        //velma.analytics='UA-74085954-1';
          </script>;

####Comment Management System  
##### How to insert disqus comment system  
1.Go to http://disqus.com and signup/login for free.  
2.After that click on the setting icon on top right corner of home page and from dropdown select `Add Disqus to site`  
![Disqus how to](http://i.imgur.com/hWnGZa3.png)  
3.After this click on `Install on your site` on the top right corner  
![Disqus how to](http://i.imgur.com/RSImt0R.png)  
4.Fill the form provided next and then click on button "Next"  
  1.  Insert your blog name in the field `site name`  
  2.  Choose a unique disqus url which will be used later to access moderation tools and site settings. This will also become your site's "shortname".  
  3.  Select the appropriate category for your blog  

Form showing after filling entries to register for a blog named "Velma"  
![Disqus how to](http://i.imgur.com/fp6kIbm.png)  
5.After that close the browser tab.  
6.Go to the admin panel and click on code injection in left side.  
7.Go to the line no 25 on blog header section and replace the velma123 with your disqus short name. // from the line.  

##### How to insert facebook comment system  
1. Go to the admin panel and click on code injection in left side.  
2. Go to the line no 26 on blog header section and delete the two // from the line.  

#### How to set social media profiles  
1.Go to the admin panel and click on code injection in left side.  
2.Go to the line no 3 to 10 on blog header section.  
3.Change the url with your social media links to the corresponding category and make sure that those lines are not prefixed with 2 forward slashes(//).  
4.In order to remove any profile just add two // to the beginning of the line.  

####Follow Buttons  
##### Facebook like button  
THe button is enabled automatically when you set the social media profile for facebook but if you want to remove the like button just remove the 2 forward slashes from line 14 and add again // in future if you want to enable them again  

##### Twitter follow button  
THe button is enabled automatically when you set the social media profile for Twitter but if you want to remove the follow button just remove the 2 forward slashes from line 15 and add again // in future if you want to enable them again  

##### Google plus follow button  
THe button is enabled automatically when you set the social media profile for Google plusr but if you want to remove the follow button just remove the 2 forward slashes from line 16 and add again // in future if you want to enable them again  

##### LinkedIn follow button  
To enable the Linkledin button remove the 2 forward slashes from line 17,18 and 19 and set the id to your profile ID on line 18  

##### Youtube subscribe button  
To enable the subscribe button remove the 2 forward slashes from line 20,21 and 22 and set the channel to you channel name in line 24  

##### Tumblr follow button  
To enable the Tumblr button remove the 2 forward slashes from line 23,24 and 25 and set the blog name to you blog name in line 24  

####Embedding Timelines  
#####Facebook Timeline
THe TimeLine is enabled automatically when you set the social media profile for facebook but if you want to remove the TimeLine just remove the 2 forward slashes from line 34 and add again // in future if you want to enable them again  

#####Twitter User Timeline  
1.Sign in to Twitter.  
2.Go to your settings and select Widgets.  
3.Click Create new.  
4.Choose the User Time(which is default selection) of embedded timeline you’d like and start to configure it:  
1. For User Timeline, enter the username of the user whose Tweets you want to display.
operators).  

4.Make sure to select Safe mode if you want to exclude sensitive content, profanity, etc.  
5.Set  height to 400, theme as light and link color to match your website. You can also configure your embedded timeline to auto-expand Tweets containing media.  
6.Click create widget and copy the code to notepad and look for data-widget-id and copy the number.  
7.Now close the tab and go to the admin panel and click on code injection in left side.  
8.Go to the line no 35,36 and 37 on blog header section and remove the // from each line.  
9.Now copy that pasted number to line 36 in place of the existing number.  

#####Instagram Feed  
1.Go to the admin panel and click on code injection in left side.  
2.Go to the line no 38,39,40 and 41 on blog header section and remove the // from each line.  
1. Go to https://instagram.com/oauth/authorize/?client_id=a525e19ee1494f158f029a78de89369e&redirect_uri=http://instafeedjs.com&response_type=token  
2. Now copy the access Token provided to line number 40 in place of that string  
3. And copy the userId to line number 39 in place of that number.  

#####Flickr Feed
1.Go to the admin panel and click on code injection in left side.  
2.Go to the line no 42,43,44,45 and 46 on blog header section and remove the // from each line.  
3.Get your Flickr ID either by idgettr.com or by clicking on your buddy icon and take out the number part  
4.Now copy the ID to line 44 in place of that numerical value  

####Newsletter  
1.Go to mailchimp.com and signup/login.  
2.Then go to Lists and click on create new list![New List](http://i.imgur.com/G2j1Xnv.png)  
3.Then Fill in the details as appropriate![Filling form](http://i.imgur.com/2CQzNMp.png)  
4.After that click on signup forms and then embedded forms ![Selecting type](http://i.imgur.com/WbX6b5N.png)  
5.After select Naked Forms and uncheck and deselct everything else than "Show only required fields"![creating form](http://i.imgur.com/PxMnGVN.png).  
6.Now Copy the code generated in the section "Copy/paste onto your site".  
7.Now open your theme folder velma and go to partials folder and then open newsletter.hbs file in notepad and delete everything inside the file and paste the code from mailchimp.  
8.Now close the tab go to the admin panel and click on code injection in left side.  
9.Go to the line no 49 to 54 on blog header section and remove the // from each line **except line 51**.  
10.In future if you want to remove the newsletter just remove // from line 51.  

####Google Analytics  
1.go to https://www.google.com/analytics/web/####home/ and click on sign up![Begin](http://i.imgur.com/ZDdiboU.png)  
2.Now fill in the form as appropriate and as shown here![Demo](http://i.imgur.com/JKcdvC0.png)  
3.Then accept the terms and condition and then you will see something like ![Main](http://i.imgur.com/kjf7aHQ.png)  
4.Now copy the tracking ID as shown in the image.  
5.Now close the tab and Go to the admin panel and click on code injection in left side.  
6.Go to the line no 56 on blog header section and remove the // and replace the tracking code.  

####Privacy policy
create a static page with url /privacy-policy in the admin panel.

####Advertisement  
1.Go to the ghost folder then content -> themes -> partials.  
2.Open the file "advertisement.hbs" file in notepad.  
3.Copy the advertisement code in the "advertisement.hbs" file.  

####Demo file

The code injected file for Velma looks like

        <script>
        	velma.url={
        		facebook:"https://www.facebook.com/RedHive-Software-623049087845699/",
        		twitter:"https://www.twitter.com/redhivesoftware",
        		tumblr:"https://www.tumblr.com/blog/redhivesoftware",
        		gplus:"http://plus.google.com/u/0/115145342026041498272",
        //		youtube:"your youtube url",
        //		linkedin:"your linkedin url",  
        		instagram:"https://www.instagram.com/velmaredhivesoftware",  
        		flickr:"https://www.flickr.com/photos/redhivesoftware/",  
        		end:true
        	}
        	velma.follow={
        //		facebook:'disabled',
        //		twitter:'disabled',
        //		gplus:'disabled',
        //		linkedin:{
        //			id:123
        //		},
        //		youtube:{
        //			channel:'Sic7VK9KUtKMgaWa5Nz71Q'
        //		},
        		tumblr:{
        			blogname:'redhivesoftware'
        		},
        		end:true
        	}
        	velma.comment={
        		disqus:'velma123',
        	//	facebook:'enabled',
        		end:true
        	}
        	velma.feed={
        //		facebook:'disabled',
        		twitter:{
        			id:'696094298215940096'
        		},
        		instagram:{
        			userId:'2899013383',
        			accessToken:'2899013383.a525e19.a119b4854c944131bbe5f6632ef76a48'
        		},
        		flickr:{
        			qstrings:{
        				id:'139052977@N02'
        			}
        		},
        		end:true
        	}
        	velma.newsletter={
        		popup:true,
        //		hide:true,
        		time:10,
        		end:true
        	}
            velma.analytics='UA-74085954-1';
        </script>

####How to change the favicon  
1.Go to the ghost folder then content -> themes -> asset.  
2.If already present then delete the file named "favicon.ico" and paste your icon file with name favicon.ico.  


####Credits

bootstrap.js / bootstrap.min.js – Bootstrap 3 - http://www.getbootstrap.com
Jquery http://jquery.com
Underscore http://underscorejs.org
Backbone http://backbonejs.org
Pixabay for Demo Images http://pixabay.com
Fitvids http://fitvidsjs.com
InstafeedJS http://instafeedjs.com
Jflickrfeed http://www.newmediacampaigns.com/blog/a-jquery-flickr-feed-plugin
FontAwesome Icons https://fortawesome.github.io/Font-Awesome/
Pacifico Google Font https://www.google.com/fonts/specimen/Pacifico
Roboto Google Font https://www.google.com/fonts/specimen/Roboto
Open Sans Google Font https://www.google.com/fonts/specimen/Open+Sans
Owl-Carousel http://owlgraphic.com/owlcarousel/
xml2json http://www.fyneworks.com

####Release  
Version 1.0.0
