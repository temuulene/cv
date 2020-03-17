## My pagedown rendered CV

I have modified [Nick Strayer's wonderful CV](http://nickstrayer.me/cv) to my own needs here.  

### Structure

This repo contains the source-code and results of my CV built with the [pagedown package](https://pagedown.rbind.io). 

The main files are:

- `index.Rmd`: Source template for the cv, contains a variable `PDF_EXPORT` in the header that changes styles for pdf vs html. 
  - `index.html`: The final output of the template when the header variable `PDF_EXPORT` is set to `FALSE`. View it at [nickstrayer.me/cv](http://nickstrayer.me/cv).
  - `temuulen_cv.pdf`: The final exported pdf as rendered by Chrome on my mac laptop. Links are put in footer and notes about online version are added. 
- `parsing_functions.R`: A series of small functions for parsing a position entry into the proper HTML format. Includes logic for removing links if needed etc..
- `gather_data.R`: Loads the data that makes up the body of the CV. Either pulls from a specified google sheet with info.
- `css/`: Directory containing the custom CSS files.