# GGPlot

ggplot is a popular library within python: see http://ggplot.yhathq.com/
As it says there:

	"Making plots is a very [repetitive]: draw this line, add these colored points, then add these, etc. Instead of re-using  the same code over and over, ggplot implements them using a high-level but very expressive API. The result is less time spent   creating your charts, and more time interpreting what they mean.
	ggplot is not a good fit for people trying to make highly customized data visualizations. While you can make some very intricate, great looking plots, ggplot sacrafices highly customization in favor of generall doing "what you'd expect".

Quote:

	ggplot has a symbiotic relationship with pandas. If you're planning on using ggplot, it's best to keep your data in DataFrames. Think of a DataFrame as a tabular data object. For example, let's look at the diamonds dataset which ships with ggplot.

Ref: http://ggplot.yhathq.com/how-it-works.html
from ggplot import *
diamonds.head()
"

http://ggplot.yhathq.com/how-it-works.html

What's interesting about the 'grammar' of graphics is that you can deal with types of plots on the same axis: first you define your plot as a variable .e.g. 'p'.
Then you use the '+' operation to introduce more complexity, incrementally, to the plots.  This abstraction is something that computing systems do in order to improve usability and intelligibility of software interfaces.  It enables a user to express different combinations in 'words', which themselves are complex ideas.
