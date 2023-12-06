# mne-shit

mindMonitor_2023-10-31--20-11-02_4625240158191494507.zip
Raw data collected while sleep deprived, after ingesting 600mg of caffiene,  and in a state of stress.

mindMonitor_2023-10-31-updated.csv
The same file but after getting rid of NANs using SQL

mindMonitor_2023-10-31-amended.csv
I found a better way of getting rid of NANs and cleaning my data using sklearn.impute, SimpleImputer
(data cleanup file)

MNEControlcomparison
Super sqeeky clean M/EEG data retrieved from a controlled enviournment. Data from a strangers brain.

data cleanup
Cleaning mindMonitor_2023-10-31-updated.csv

main file 
Reading csv, converting to fif, setting bandpass filter, visualizing data & unit tests. This file uses data that I have collected from my own brain.
I am comparing the plotting output of my main file and the MNEControlcomparison file. 
