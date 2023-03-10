# Shopify Dawn - Reduced
This theme is a reduced version of Shopify's Dawn version 8.0.0-rc.
It's a starting point for projects where the ability to change theme settings isn't desireable.
Most of the settings have been stripped from settings_schema.json, and anything accessing them from liquid files has been hard coded to the default values.
Some useful properties remain in theme.liquid and have been hard coded.

## Colours
Colours are defined in theme.liquid. The colour name is in the base property name for readability, rather than Dawn's flexible naming convention.
Colour classes have also been changed from the 'background-1' naming convention to the name of the colour, again for readbility throughout the liquid files.
Values within section schema settings have been updated to include the new colour classes.
A global search/replace to change the classes and schema values is obviously recommended when changing the colours.

## Fonts
The font is being loaded through Google Fonts as Shopify's font picker has been removed. If using fonts locally, remove the google preconnect and font stylesheet from theme.liquid. 