# The Evolution of Hip-Hop

**DSC160 Data Science and the Arts - Midterm Project Repository - Spring 2020
Project Team Members:
● Dan Ngo,** ​ **dmngo@ucsd.edu
● Justin Lee,** ​ **jul290@ucsd.edu
● Jaskaranpal Singh,** ​ **jas137@ucsd.edu
● Iman Nematollahi,** ​ **imnemato@ucsd.edu
● Andrew Shin,** ​ **sgs008@ucsd.edu**

## Abstract ​ :

As is the case with many young people today, hip-hop has played a significant role in the
lives of the members of our group; we see and hear it everywhere, constantly shaping today's
culture. Newer hip-hop artists can be seen experimenting with new styles all the time as they try
to break down the boundaries set by those who came before them and attempt to carve out their
own legacy within the music industry. As such, the hip-hop of today, which still retains much of
the core characteristics of what defines a song as being “hip-hop”, sounds markedly different
from the hip-hop of the last decade and beyond. In fact, in recent years, hip-hop artists have also
gained a more direct influence on mainstream culture with their unprecedented levels of fame
allowing them to collaborate with huge brands such as Travis Scott’s collaboration with Nike or
Kanye West’s with Adidas (which is a multi-billion dollar business venture). With all of these
changes happening within hip-hop culture, it only makes sense that this would have an affect on
the genre of hip-hop itself. All of our group members love to listen to hip-hop music; however,
we can all agree that the style and sound of hip-hop has changed drastically throughout time.
Therefore, we have decided to base our project around our favorite genre and to analyze its
transition in style over the years. Our group is curious as to what core differences exist between
older and newer hip-hop and we hope that our analysis will be able to point out some key
differences between these generations of music. Specifically, we will be analyzing a set of
hip-hop songs that were popular in the 90’s and compare them with a set of hip-hop songs that
are popular now.
Hip-hop, in each of its eras, has had a distinctly unique sound. By studying how the genre
of hip-hop has changed musically, specifically in terms of beat/sound selection, we will attempt


to resolve the question of how hip-hop has changed in the past few decades. We will first try to
establish whether there really exists a significant sonical difference between the music from the
90’s and from the 10’s. This will mainly be explored through the use of chromagrams and
Fourier transforms, which were demonstrated in class. The Fourier transform will be able to tell
us which notes were most commonly used in each era of hip-hop and the chromagrams will be
able to tell us which pitches were the most prevalent. To ensure that our results are as meaningful
as possible, we will also attempt to limit the effect of confounding variables by comparing
hip-hop songs from two separate geographical regions, the West Coast and the East Coast. Since
even people unfamiliar with hip-hop are able to recognize that the hip-hop music that we listen to
varies extensively depending on where the artist is from, we believe that offsetting our results for
such a factor will allow us to generate the most accurate results. In summary, our objective in
this project is to see whether we can identify any significant differences in the styles of hip-hop
of the 90’s and of today, with a secondary focus on determining whether geography matters as
well.

## Data ​ :

For our analysis, our dataset will consist of four sets of 10 hip-hop songs, 20 from the
90’s and 20 from the 10’s. Of the 20 songs that belong to each era, 10 of the songs will be from
artists from the West Coast and 10 of the songs will be from artists from the East Coast. Thus,
our data set will be divided into four subsets: 90’s West Coast hip-hop, 90’s East Coast hip-hop,
10’s West Coast hip-hop, and 10’s East Coast hip-hop. Separating our dataset into these smaller
individual subsets will allow us to get a better idea of the differences between the styles of
hip-hop from the varying decades and geographical regions. Also, the songs that we selected for
our analysis are the top hip-hop songs relevant to that category and were downloaded from
YouTube and then converted into mp3 files.

### 90’s West Coast Hip-Hop songs ​ :

```
1) It Was A Good Day ​ - Ice Cube (​ Released: ​ ​1992)
https://www.youtube.com/watch?v=VA_P8DREazc
2) Straight Outta Compton ​ - NWA (​ Released: ​ ​1988)
https://www.youtube.com/watch?v=TMZi25Pq3T
3) The Next Episode ​ - Dr. Dre ft Snoop Dogg, Kurupt & Nate Dogg (2000)
https://www.youtube.com/watch?v=QZXc39hT8t
4) Boyz-N-The-Hood ​ - Easy-E (​ Released: ​ ​1987)
https://www.youtube.com/watch?v=zDQoF6GyXas
```

```
5) Gin N Juice ​ - Snoop Dogg (​ Released: ​ ​1993)
https://www.youtube.com/watch?v=OKGJOtRaqMg
6) All Eyes On Me ​ - 2Pac (​ Released: ​ ​1996)
https://www.youtube.com/watch?v=zSzaplTFagQ
7) No Vaseline ​ - Ice Cube (​ Released: ​ ​1991)
https://www.youtube.com/watch?v=bvRc7pwnt0U
8) California Love ​ - 2Pac ft Dr. Dre (​ Released: ​ ​1996)
https://www.youtube.com/watch?v=J7_bMdYfSws
9) Nuthin But A G Thang ​ - Dr Dre ft Snoop Dogg (​ Released: ​ ​1992)
https://www.youtube.com/watch?v=6xjRdBjmePQ
10) Regulate ​- Warren G (​ Released: ​ ​1994)
https://www.youtube.com/watch?v=1plPyJdXKIY
```
### 90's East Coast Hip-Hop songs ​ :

```
1) Brooklyn's Finest ​ - Jay-Z ft. Notorious B.I.G (​ Released: ​ ​1996)
https://www.youtube.com/watch?v=4o24e7MnblU
2) The World is Yours ​ - Nas (​ Released: ​ ​1994)
https://www.youtube.com/watch?v=_srvHOu75vM
3) Juicy ​ - Biggie Smalls (​ Released: ​ ​1994)
https://www.youtube.com/watch?v=7Y8VPQcPHhY
4) C.R.E.A.M. ​ - Wu-Tang Clan (​ Released: ​ ​1993)
https://www.youtube.com/watch?v=ecRs1sWZIL
5) The Choice is Yours ​ - Black Sheep (​ Released: ​ ​1991)
https://www.youtube.com/watch?v=FXQvvv6rFJk
6) Ain't the Devil Happy ​ - Jeru Tha Damaja (​ Released: ​ ​1994)
https://www.youtube.com/watch?v=qkJpjc3IU0M
7) Survival of the Fittest ​ - Mobb Deep (​ Released: ​ ​2000)
https://www.youtube.com/watch?v=i9ZykEJuFrI
8) Shadowboxin' ​ - GZA (​ Released: ​ ​1995)
https://www.youtube.com/watch?v=Y_JS051vquo
```

```
9) Dangerous Minds ​- Gravediggaz (​ Released: ​ ​1997)
https://www.youtube.com/watch?v=B2eDNo6PX6Y
10) Break Ya Neck ​- Busta Rhymes (​ Released: ​ ​2001)
https://www.youtube.com/watch?v=PAr0YlIv1zw
```
### 10’s West Coast Hip-Hop songs ​ :

```
1) Bubblin ​ - Anderson Paak (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=7PmUtmfTmbg
2) Thotiana ​- Blueface (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=1bBZMPER85I
3) Wow Freestyle ​ - Jay Rock ft. Kendrick Lamar (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=GTe57jQX5Eg
4) M.A.A.D. City ​ - Kendrick Lamar (​ Released: ​ ​2012)
https://www.youtube.com/watch?v=10yrPDf92hY
5) Rack City ​ - Tyga (​ Released: ​ ​2011)
https://www.youtube.com/watch?v=slmfu0IP9Z
6) The Box ​ - Roddy Rich (​ Released: ​ ​2019)
https://www.youtube.com/watch?v=uLHqpjW3aDs
7) Bands ​- Shoreline Mafia (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=l41LN8QJVzo
8) Calvin Cambridge ​- SOB x RBE (​ Released: ​ ​2017)
https://www.youtube.com/watch?v=U-_XJkIqWPs
9) Yonkers ​ - Tyler The Creator (​ Released: ​ ​2011)
https://www.youtube.com/watch?v=XSbZidsgMfw
10) Suu Whoop ​ - YG (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=Yit3CnDL23I
```
### 10’s East Coast Hip-Hop songs:

```
1) Bad and Boujee ​ - Migos ft. Lil Uzi Vert (​ Released: ​ ​2016)
https://www.youtube.com/watch?v=S-sJp1FfG7Q
2) Lucid Dreams ​ - Juice Wrld (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=mzB1VGEGcSU
```

```
3) Digits ​ - Young Thug (​ Released: ​ ​2016)
https://www.youtube.com/watch?v=I7w9otyiE9g
4) Drip or Drown ​- Gunna (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=BYZrDgavkpU
5) Everyday ​ - A$AP Rocky ft. Rod Stewart, Miguel, Mark Ronson (​ Released: ​ ​2015)
https://www.youtube.com/watch?v=UtZBA1bVbcs
6) I Get The Bag ​- Gucci Mane ft. Migos (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=uo14xGYwWd
7) No Heart ​- 21 Savage (​ Released: ​ ​2017)
https://www.youtube.com/results?search_query=no+heart
8) Since When ​ - Young Nudy ft. 21 Savage (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=Nl0PCrQiFok
9) Wokeuplikethis ​ - Playboi Carti ft. Lil Uzi Vert (​ Released: ​ ​2018)
https://www.youtube.com/watch?v=REmZhFKmOmo
10) Work Out ​ - J Cole (​ Released: ​ ​2011)
https://www.youtube.com/watch?v=UWlibNTrg
```
## Code ​ :

Our code is split among four separate notebooks, with each notebook dedicated to one of
our four subsets of hip-hop music: 90’s West Coast hip-hop, 90’s East Coast hip-hop, 10’s West
Coast hip-hop, 10’s East Coast hip-hop. The notebooks all generally follow the same format and
display the same types of information, but they differ in that each contains analysis for a
different set of 10 songs by varying artists of that category. This allowed us to easily compare the
results for the different subsets and to see what significant distinctions could be made between
each of the four individual categories.
The first step in our code was to load the 10 songs of the associated subset into the
notebook. We decided to take a 1-minute clip of each song, all of which were offset by a minute
(so 1:00 - 2:00 for every song); this would allow us to ignore the intros of the songs and would
let us skip to the more musically-dense portions of the songs, which is what we aim to analyze in
this project. We then generated all of the clips of music as playable audio to encourage the user
to listen to each set of songs and to get an idea of what each category generally sounds like. We
commented out these audio lines to save storage; they should be uncommented when the user
wants to listen. Following this, we also calculated several different measurements and produced


some visualizations for analysis, such as wave plots, Fourier transforms, chromagrams, zero
crossings, and spectrograms. In the notebooks, we specify where each measurement/visualization
is being generated, and all of the outputs for that section are preceded by a corresponding song
title. All of the notebooks should produce clear and easy-to-follow output if run sequentially
from top to bottom.

## Results ​ :

The documentation of the output of our results is included in the notebooks that contain
our code. Using the results found in each of these notebooks, we compared the different
measurements that we calculated across the different categories. Our results gave us a number of
interesting insights into the relationship between East Coast and West Coast hip-hop, both during
the 1990’s and 2010’s.
Based on what we found using the Fourier transform, 1990’s East Coast hip-hop songs
seem to feature a wide variety of notes, with the most common notes being G2 and F10. Looking
at the chromagrams of all the samples, the loudest portions, in general, tend to stay within the D,
F and G pitches. Zooming into these chromagrams, however, shows that many of the songs tend
to follow similar pitch distributions, with five of the ten songs having dense, straight red “band”
patterns spanning roughly 3 half pitches that persist throughout the entire song, and with four of
the ten songs having a sinusoidal wave pattern spanning roughly 9 half pitches. The 90’s hip-hop
song, “The Choice is Yours,” features the widest variation in pitch classes with the total intensity
of the song being dispersed across all 12 half pitches. We also found that, on average, the
samples have 124,713 zero crossings, with the range of zero crossings being 85,987 - ​170,486​.
Chromagram of “Survival of the Fittest - Mobb Deep” showing what a “band” would look like


Chromagram of “The Choice is Yours - Black Sheep” showing a large dispersion of pitch presences
1990’s West Coast hip-hop featured a lot of G1 and F10 notes, demonstrated through the
Fourier transform. The chromagram of each song illustrates a consistent use of the D and G pitch
classes. The chromagrams also show a “band” pattern on many of the songs, generally near G,
which demonstrates the consistent use of the G pitch class throughout this era’s hip-hop music.
One of the most prominent of these “bands'' is shown in the chromagram for “Nuthin But a G
Thang” where we can see a long red line spanning only the G pitch class throughout the entire
clip. The number of zero crossings for this specific era and location was also very high; the
average total number of zero crossings being 163,882. These zero crossing values help to
identify beat detection and to give us a better understanding of different beats patterns in
different songs. For instance, “Regulate” had a significantly lower number of zero crossings
(68,977), which makes sense as the song is much more relaxed and slow than the others.
Looking at the spectrogram for “Nuthin But a G Thang,” we can see a consistent intensity
throughout the song, which is similar to the style of many of the other West coast hip-hop songs
from the 90’s.


Looking at the Spectrogram for “Regulate” we can see that it is an outlier in this subset as it
depicts a much calmer style of hip-hop. This may explain why the zero crossing rate was so low
compared to the other songs.
2010’s East Coast hip-hop, according to our findings, heavily featured the use of the D#
and F10 notes. Analyzing the selected songs using the Fourier transform, we were able to
identify these two notes as being especially prevalent in the music of this era and area. The
results of our chromagrams also indicated prominent usage of the E, F, and D pitch classes. We
found that for this subsection of our data, while most of the chroma charts were heavily banded
and formed straight lines, 3 out of our 10 songs featured heavy variation among the pitch classes
throughout the entirety of the song, an example of which can be seen below. We also found that
the ten chosen songs had an average of 83,741 zero crossings.


2010’s West coast hip-hop, on the other hand, featured some use of the A#0 and G
notes, though there was no clear pattern as to which notes were most prevalent. There was a
similar issue in determining which pitch classes were most common while looking at the
chromagrams. This may be due to the fact that there is much more variance in the hip-hop music
of this era and region than of the other eras and regions analyzed. Also, the number of zero
crossings for 2010’s West coast hip-hop was higher than the number of zero crossings for 2010’s
East coast rap, averaging at ​122,558 zero crossings.
We found distinct differences between East Coast and West Coast hip-hop in the 1990’s.
Using the Fourier Transformation, we found that East Coast hip-hop has a much more dispersed
usage of pitches across songs with the mode of the samples being G2 (2 occurrences), while the
West Coast heavily featured G1(4 occurrences) as the dominant note, with G#1 occurring twice.
Upon looking at the chromagrams, one can also see that the intensity of pitches in East Coast
hip-hop are much more defined around the center of the band, while West Coast hip-hop has a
much more dispersed presence of pitches.
Chromagram of “Dangerous Mindz - Gravediggaz”​ **(East Coast)** ​ band with smaller spread
Chromagram of “Straight Outta Compton - NWA”​ **(West Coast)** ​ showing band with larger dispersion of pitches


We found some clear differences between the two regions we analyzed during the 2010s.
From the chromagrams of either region, we can see that East Coast hip-hop songs used the D#
and F10 notes quite heavily, while the notes used in West Coast songs were more varied. West
Coast songs also had less striation within their chroma vectors than East Coast songs.

## Discussion ​ :

When analyzing the results of the metrics calculated for the 90’s and 10’s West/East
Coast hip-hop, we noticed some differences between the categories that might explain the
transition of musical style throughout the decades. Between the two geographic regions of the
90’s, we see that there was a similar use of notes and pitch classes, primarily of D’s and G’s.
Within our samples, we also see that 90’s West Coast hip-hop has a 29.7% larger zero crossing
rate on average than 90’s East Coast hip-hop, which demonstrates that West Coast hip-hop back
then was commonly more “noisy” as a result of their use of more complex beats. Pitch classes
throughout hip-hop music in the 90’s were more likely to be “banded” as well, meaning that
certain notes, most commonly G, were consistently more prominent than others throughout the
song. This invariability within 90’s hip-hop songs may be due to the fact that hip-hop beats
during this time tended to be much more repetitive, whereas today, the beats tend to change more
as the song develops.
As we shifted our analysis to focus on the 2010’s, we noticed that there was a more
diverse group of notes and pitch classes used in the songs from both the East and the West
coasts. Looking at the chromagrams for both regions, we see that there is much less
“banded-ness” around certain notes and pitch classes as well. This can likely be attributed to
these subsets of hip-hop songs having a more diverse and complex structure and incorporating a
larger number of different combinations of pitches than the hip-hop songs in the 1990’s subsets.
This rise in variation between the generations may be due to the fact that music nowadays is
typically produced using software, as opposed to the 90’s when beats had to be compiled using
actual instruments. Because technology has advanced so rapidly throughout the years, new
software and tools are constantly being made available to artists everywhere, which allows them
to explore their creativity and individual styles more freely. As such, artists are able to
experiment with all kinds of different music samples, many of which are not of physical
instruments.
And lastly, we noticed that the zero crossing rates for hip-hop songs of the 10’s were
drastically smaller than the zero crossing rates for hip-hop songs of the 90’s. This decrease over
time can probably also be attributed to the advent of new music production and editing software.
This is because these tools now allow for creators to manipulate audio waves so as to minimize
the number of zero-crossings, which is related to beat detection within songs. Furthermore, in


both the 90’s and the 10’s subsets, we can see once more that hip-hop songs from the West coast
tend to have a significantly higher average zero crossing rate than hip-hop songs from the East
coast, emphasizing yet again the point that hip-hop songs of the West coast, in general, typically
are “noisier” and are more complex. This matches our intuition as hip-hop songs from the West
coast are commonly less lyrically complex but more complex in terms of the beat, whereas
hip-hop songs from the East coast are commonly more lyrically complex but have a less complex
beat.
Though originally we planned to take both a sonical and a lyrical approach, we ultimately
decided against it because we determined that the results of a sonical approach would be more
meaningful. We also believed that a sonical approach would allow us to focus more on the music
itself, rather than on trying to sort through and discern significant keywords or phrases in the
lyrics of the songs. However, this does not mean that an analysis of lyrical data would not
produce significant outcomes; it would definitely be interesting to see what kinds of results could
be generated by such a study. As such, one possible extension of this project would be to take the
lyrical approach and see what conclusions can be made. Another possible extension would be to
create a classifier to distinguish between old school hip-hop and new-school hip-hop by training
the models on features such as MFCC’s or spectral centroids.


## Team Roles ​ :

**Iman** ​ ​ **Nematollahi** ​: 90’s West Coast Notebook, Data, Code, part of Results, part of Discussion
**Jaskaranpal Singh:** ​10’s East Coast Notebook, Data, Code, part of Results, part of Discussion
**Justin Lee:** ​10’s West Coast Notebook, Data, Code, part of Results, part of Discussion
**Dan Ngo:** ​90’s East Coast Notebook, Data, part of Results, part of Discussion, Formatting
**Soon Gi Shin** ​: Data, Code, Abstract, part of Results, part of Discussion, Proofreading

## Technical Notes and Dependencies

Required libraries/import statements as mentioned in the ipynb notebook files.

## Reference

### ● Personal Hip-Hop Knowledge/Passion

### ● https://harvardpolitics.com/covers/evolution-rap/​ - influence of the internet

### ● Basic audio feature notebook

### ● Advanced audio feature notebook

