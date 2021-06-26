# Photo Quality Analysis

Please see the .ipynb for details; I've copy-pasted the results below:

I set out to take a silly, empirical take on a subjective and unanswerable question - what makes a photo good?  

Here we have limited n, ambiguous features, noisy labels/ratings... mostly everything is out of our control. Still, it's fun to try to answer hard questions with limited data ;)  


### Methods  

I attempted to predict two outcomes - one a subjective continuous photo quality rating, the other a binary successful or unsuccessful photo rating. Theris some difficulty with the continuous ratings due to bimodality, a result of the sampling technique (see below). However, the binary outcome gives up some information, since we lose the small variations of "success" and "non-success" within generally successful or unsuccessful photos as classes. (A photo that's I call "successful" may vary from a rating of around 80 to 100, and an unsuccessful one from about 50 to 70.)  

Photo features were derived from metadata where possible with additional features added by hand. Ratings were, of course, by hand.  

Photos were sampled in a two-step process: first I chose the approximately 130 highest-rated photos from my photo library. Then I also sampled another approximately equal number of photos uniformly random with respect to photo index by time. That is, in simpler terms, I just chose every 200th photo.  

### Results  

Unsurprisingly, most effects are pretty weak. The only really strong effect was a positive effect of the "golden hour" near sunset. There are some weaker effects in favor of medium format film (but I shoot much more conservatively with this since it's expensive per-frame) and landscape photos (most of what I shoot "seriously" - as opposed to portraits, events). (That is, there is pretty profound selection bias that I _attempt_ to control for but am unlikely successful in doing so!

