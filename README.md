# Sparkify user churn prediction with Pyspark



### Table of content
---------------
* [Motivation](https://github.com/IamGr0o0t/Sparkify_User_Churn#motivation)
* [Installation](https://github.com/IamGr0o0t/Sparkify_User_Churn#installation)
* [Software versions](https://github.com/IamGr0o0t/Sparkify_User_Churn#software-versions)
* [File descriptions](https://github.com/IamGr0o0t/Sparkify_User_Churn#file-Descriptions)
* [Results and Findings](https://github.com/IamGr0o0t/Sparkify_User_Churn#results-and-findings)
* [Licensing, Authors, Acknowledgements](https://github.com/IamGr0o0t/Sparkify_User_Churn#licensing-authors-acknowledgements)

### Motivation
---------------
Sparkify is a music streaming platform similar to Spotify. By predicting likelyhood of an individual leaving the platform, can save companies like Sparkify millions in revenue and this project tries to do just that

### Installation
---------------
Most of the packages used are installed via most recent conda distribution.
```bash
conda 4.8.3
```
If you wish to install some other packages please feel free and do it with conda-forge. 
```bash
conda install -c conda-forge (Insert Package Here)
conda install -c conda-forge pyspark
```
### Software versions
---------------
* Anaconda version == 4.8.3
* Python version == 3.7.6
* pandas version == 1.0.1
* Numpy version == 1.18.1
* matplotlib version == 3.1.3
* seaborn version == 0.10.0
* pyspark version == 2.4.5

### File descriptions
---------------
There is only one data file and it is a small subset (128Mb) of much larger data available online (12Gb)
* Data</br>
!IMPORTANT file is missing because it exceeds max file capacity of 100Mb
|- mini_sparkify_event_data.json (user log data available on Sparkify platform.)</br>


* Sparkify_churn.ipynb (jupyter notebook file containing all python script needed for churn analysis and churn predictions)
* Sparkify_churn.html (html version of jupyter notebook file)

### Results and Findings
---------------
Main questiond answered:
- What are the most common activities users perform on Sparkify platform?<br>
    By excluding NextSong from results we have better view on user interaction with the platform. People are very generous with liking their music compared to dislikes given.<br>
- What a key personality behavior traits that distinguish people who churn and not churn?<br>
    Total number of songs played is larger in users who stay loyal to the platform.<br>
    Users who churn are much more generous with dislikes given compared to likes given.<br>
    On average number of songs listened by session, not churn cases are much more active compared to users who left the platform.<br>
- Is there any important gender discrepancy?<br>
    Surprisingly there are more male users than female.<br>
    Although the difference is not significant, male users are more likely to leave the platform.<br>
    On average female users interact with platform more. We can see that in number of songs, songs liked and disliked.<br>
- How well can we predict if a given user might or might not leave Sparkify platform?<br>
    Our final model with best parameters has some impressive results with .88 accuracy and .87 f1-score<br>
- When to send our marketing communication to people who most likely are to churn?<br>
    To maximize likelihood of user interaction with our marketing campaign, we should send it during afternoon hours on any workday.<br>
### Licensing, Authors, Acknowledgements
---------------
The dataset provided i part of Sparkify platform.<br>
Thanks to [Udacity.com](https://classroom.udacity.com) for an amazing Data Science course.
