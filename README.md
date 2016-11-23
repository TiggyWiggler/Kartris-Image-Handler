# Kartris-Image-Handler
Replace ASPX fed images with ASHX images

The current ~/Image.aspx implements the entire page lifecycle, and also delivers the image as a HTML document, not as an image. 
This negatively impacts the way in which search engines view the images (as they do not see them as images) and also has a performance 
impact as the entire page lifecycle is unneccessarily loaded up. This handler rectifies this problem because handlers do not implement
the entire page lifecycle. 

Extra care had to be taken due to the cache settings in handlers requiring manual settings, but I believe this has been set correctly. 
