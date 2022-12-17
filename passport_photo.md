# Create passport photo 4x6

## Steps

* From your gimp "Toolbox", click the "Rectangular Select" tool. (Ensure that the "Fixed Aspect Ratio" is unticked).  Draw a small rectangle surrounding your face. In the left hand-pane, choose Size, Enter width=350 px and height=450 px.  (or a ratio of this) and then select "Fixed Aspect Ratio".  You will see a rectangle area in the image to be adjusted accordingly. (Please recheck the Aspect ratio is 350 x 450 as sometimes, GIMP will reset it)
* From GIMP Menu  Image -> Crop to Selection.
* Now we will resize the image.  From GIMP menu,  Image -> Scale Image and select width=750 px. The height should become 964 px.  If its not becoming 964, something went wrong. Start again
* Open a new GIMP window (File -> New), and specify width = 814 px, height = 1092 px, and specify "fill with background colour" as below.
* This will ensure correct margins are left for the image before duplicating them. Copy (Control-C) and paste(Control-V) into new window. Click on the "white" border surrounding your photo, so that all layers are merged. 
* Now click on the white border. Then Select Filters -> Map -> Tile from GIMP window.  "Tile to new size", then  disconnect the chain symbol (by clicking on it) and set the width = 3256 px & height = 2184 px
* Ensure the "Create New Image" box is ticked. Result should have 8 photos (as shown below)
* Save the result as a new file with jpg extension, and with no-compression i.e. set to 100%. Please ensure no compression is done for quality photos. (In newer GIMP2, you can do "File -> Export To  ", then save it as with jpg extension with "passportTile.jpg")

