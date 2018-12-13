Proper use of IMG tags

SRC Paths
  Images should NEVER be hardcoded for the paths. URLs and Directory locations should be dynamic as to make them available no matter the location of the home directory. This helps a lot with local development so that it still works when uploaded to a live server.

ALT prop
  The required alt attribute specifies an alternate text for an image if the image for some reason cannot be displayed (because of slow connection, an error in the src attribute, or if the user uses a screen reader). The alt description is also very helpful for search engines. Search engines have a hard time figuring out what the content of an image actually is. They are getting better at it, but identifying the subject of a photo or picture is extremely difficult. So search engines rely on the alt description to know what is actually in a picture (they also use the file name and other attributes). Additionally, in Google Image Search, the alt description is actually shown to the user.

Read more: https://html.com/attributes/img-alt/

IMG props
  When using an IMG tag, remember to use the alt, width, and height prop values. This is for a combination of reasons. Height and width are very important for performance. When an IMG tag is used and does not have those values set, it has to renders the whole image, then once done will figure resizing and such via CSS statements. In turn, this causes multiple renders of the same image and in turn, you lose performance. By setting these values, you end up with a single full render, then a resize. 

Ex.
	<img src=”image.png” alt=”This is a test image.” width=”300” height=”300”>

***NOTE: the width and height values will assume px values only, though do not use the px portion and will not allow auto.
