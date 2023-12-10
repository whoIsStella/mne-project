# mne-project

mindMonitor_2023-10-31--20-11-02_4625240158191494507.zip
This raw data was collected on Halloween the day after pre- Halloween activities. I was sleep deprived because of these activities and I had also just gotten off of work, ( 11am - 7pm ). Throuout the day I had injested around 600-650mg of caffiene to get me through work. I was also in a state of stress. I chose this day because I knew that theses factors would invoke a response in my EEG reading when weraing the MUSE headset. I figured that it was possible to pick up some small epileptic activity with theses factors present.

mindMonitor_2023-10-31-updated.csv
I kept getting errors in MNE so I figured that it was my data. 
Because I am using the mind equvelent of a FitBit, there was a lot of noise contaminating my data. I tried to clean it using SQL
but I did not have the patience for the SQL enviournment in VS Code and I did not have time to download SSMS. I have it on another computer but it's at another apartment. My partner did have SSMS on his computer so I sent him the file.

mindMonitor_2023-10-31-amended.csv
I found a better way of getting rid of NANs and cleaning my data using sklearn.impute, SimpleImputer
(data cleanup file)
I wanted my data to be even cleaner so I used sklearn to get rid of NANs and other values that shouldn't be there.

MNEControlcomparison
This was a library of super sqeeky clean M/EEG data retrieved from a controlled enviournment. This particular dataset from this library contains small events.

data cleanup
This file as seen above cleaned mindMonitor_2023-10-31-updated.csv

main file 
Reading csv, converting to fif, setting bandpass filter, visualizing data & unit tests. This file uses data that I have collected from my own brain.
I am comparing the plotting output of my main file and the MNEControlcomparison file. When my data was plotted, there did seem to be a spike in activity. It was an interesting comparrison with the control data.
To execute the unit tests use python -m unittest -v big_ol_python_project.py
