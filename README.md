# jHeatmap
Java heatmap generator. Converts matrix of real numbers to graphic heatmap. Originally designed for genomics usage.

## Options
Usage: java -jar jHeatmap.jar -m [Matrix.file] [Options]
-----------------------------------------
Required Parameter:
Matrix file:		-m

Supported Options:
Color RGB comma-delimited:	-C	(Default 255,0,0)
Starting row:		-r	Default start at row index 1
Starting column:	-c	Default start at column index 2
Pixel height:		-h	Default 500
Pixel width:		-w	Default 200
Scaling type:		-s	treeview (default), bicubic, bilinear, neighbor
Quantile thresholding:	-q	Default 0.9
Absolute thresholding:	-a	Default off, overrides quantile parameter
Output path:		-o	Default current directory
File ID:		-f	Default based on Sample BAM filename
Help:			-H	Print this message

### Example
java -jar jHeatmap.jar -m CTCF_sense.cdt
