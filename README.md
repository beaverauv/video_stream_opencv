Package for viewing camera feed / opencv feed and saving it (not yet)


Jetson should have everything it needs already so you just need to clone this repo onto your machine



To run on jetson:

	roslaunch video_stream_opencv camera.launch



To view feed:

	rosrun video_stream_opencv view_feed.py

	or 
	(if machine doesn't have package)

	rosrun image_view image_view image:=/camera/image_raw



To view feed and save it:
	
	I have not figured out how to do this yet but someone should feel free to try it's more complicated than I expected





	 

I haven't written anything for viewing the opencv feed yet either as we don't really have a feed to view


There are a few different options do go about this though  and they're all pretty simple

	
	We could have the Jetson send its opencv images but that just feels like more work for it...

	I think the best way to go about it is to paste in our vision code to a copy of the view_feed.py file

		This method is really simple and makes are macs do work instead of the jetson but obviously it's up to y'all
