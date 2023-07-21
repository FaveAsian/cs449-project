Score 6/8

Great work so far! You answered many of my questions during our meeting, but I’d still like you to write those up into your proposal and rewrite some of your goals in terms of what you want to try, rather than what accuracy/performance you hope to achieve. You have a week to resubmit this for full points.

Essential goals:
-	Logistic regression sounds good as a baseline. Decision trees might not be worth the extra effort; they also require a bit of fine-tuning and typically aren’t great with image data.
-	Getting your dataset set up for classification will also be nontrivial, so this is fine for essential goals.

Desired goals:
-	Can you provide more specifics on how you hope to preprocess/label Evanston photos? Are those already (or easily) segmented into the same resolution, zoom, and image size? Do you have labels for what the image contains, or will you need to manually label those? Are all photos taken during the same season / time of year?
-	-> We discussed this in our meeting and you mentioned that getting the data is easy via Google Maps, but you would likely have to manually label the images. We also discussed that it could potentially be interesting to look at differences in seasons (e.g., snow, foliage) between Google queries and the training data.
-	Can you provide more specifics about what hyperparameters you want to consider tweaking and roughly what values you want to try? In general, there are infinitely many values you could consider, so it’s helpful to give yourself a starting point to explore and then see how to adjust those.

Stretch goals:
-	Try not to frame these goals in terms of accuracy; while it would obviously be great to meet or exceed the accuracy of published work, that may be outside your control (e.g., due to dataset and computational limitations). Rather, what specifically do you want to try to adjust in order to improve the accuracy of your model? As one possibility, consider trying to make use of pretrained models that may have been trained on other, larger satellite datasets.
-	Potential pretrained model to use: https://huggingface.co/blog/fine-tune-clip-rsicd , 
-	GAN approach sounds good; can you provide a bit more specifics on how you want to make your model more robust? You mentioned the plan was to retrain your model with a dataset containing perturbed images. Super-stretch goal: adversarial model where we generate new images that.
