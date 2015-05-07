# MarconiLab.github.io

Source: http://community.thingspeak.com/forum/announcements/thingspeak-live-chart-multi-channel-second-axis-historical-data-csv-export/

Here is a HTML JavaScript web page to display multiple series and channels in real time.
http://forum.arduino.cc/index.php?action=dlattach;topic=213058.0;attach=66726
http://forum.arduino.cc/index.php?action=dlattach;topic=213058.0;attach=66752
You must edit the page source/ JavaScript to enter your channel information.
If you have lots of series, it is helpful to click the "Hide All" button, and then click on the series names you are interested in to show them. Clicking and dragging vertically on the chart will select a range to zoom in to.
Check the "Update Chart" checkbox to enable realtime charting. With more than about 8 channels, this causes ThingSpeak to cache and delay the data, so I have it unchecked.
It also features buttons to load historical data 8000 points at a time. Select which channel you want to load, and how many sequential loads to try. Then click the "Load More Historical Data" button. Loading too much data causes ThingSpeak to first delay the data, and then (error 404) refuse to return data. After ten loads or so, I often cannot load any more data.
The three bars export button at the top right has an option to download a .csv file containing the data from the chart.
This is public domain. Please post upgrades on the Arduino forum thread. (too bad this forum doesn't support posting files)
http://forum.arduino.cc/index.php?topic=213058.0
The navigator could be dramatically upgraded to provide complete access to your historical data with smaller data downloads if ioBridge were to change the Average function so it would return 8000 points, instead of averaging 8000 points. http://community.thingspeak.com/forum/thingspeak-api/daily-average1440-parameter-purpose-defeated-by-results-limits/
The charting library is called HighStock. It is awesome! HighSoft, the owners say, "Do you want to use Highstock for a personal or non-profit project? Then you can use Highchcarts for free under the Creative Commons Attribution-NonCommercial 3.0 License. "
