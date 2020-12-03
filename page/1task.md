---
layout: page
title: Data and Tasks
permalink: /Task/
icon: database
type: page
---
* content
{:toc}

<span style="font-size:16px">All data and code can be accessed in 
<a href="https://github.com/indolem/indolem" target="_blank">IndoLEM Github Account</a> &#128522; &#128522;</span>

- - - - - - - - - - - - -
<span style="color:#233279; font-size:18px">&#9830; Morpho-syntax and Sequence Labelling</span>

##### **Part-of-speech tagging**
<span style="font-size:15px">We use the Indonesian POS tagging of <a href="https://ieeexplore.ieee.org/document/6973519">Dinakaramani et al. (2014)</a>, 
and 5-fold partitioning of <a href="https://arxiv.org/abs/1809.03391">Kurniawan and Aji (2018)</a>. Train/Dev/Test
distribution is 7,222/802/2,006.</span>

##### **NER**  
* <span style="font-size:15px">NER UI (Universitas Indonesia) by Fachri (2014) with training/dev/test distribution:
1,530/170/425.</span>
* <span style="font-size:15px">NER UGM (Universitas Gajah Mada) by Gultom and Wibowo (2017) with Train/Dev/Test ditribution:
1,687/187/469.</span>

##### **Dependency Parsing** 
<ul style="font-size:15px">
<li> UD-Indo-PUD: 1,000 sentences of UD-Indo-PUD (<a href="https://www.aclweb.org/anthology/K17-3001/">Zeman et al., 2018</a>), and we use the corrected version by  <a href="https://github.com/ialfina/revised-id-pud">Alfina et al. (2019)</a></li>
<li> UD-Indo-GSD: 5,593 sentences of UD-Indo-GSD (<a href="https://www.aclweb.org/anthology/P13-2017/">McDonald et al., 2013</a>)</li>
</ul>
- - - - - - - - - - - - -
<span style="color:#233279; font-size:18px">&#9830; Semantic Task</span>

##### **Sentiment Analysis**  
<span style="font-size:15px">This dataset is based on binary classification (positive and negative), with distribution:</span>
<ul style="font-size:15px">
  <li>Train: 3638 sentences</li>
  <li>Development: 399 sentences</li>
  <li>Test: 1011 sentences </li>
</ul>
<span style="font-size:15px">The data is sourced from 1) Twitter (<a href="https://www.researchgate.net/publication/321757985_InSet_Lexicon_Evaluation_of_a_Word_List_for_Indonesian_Sentiment_Analysis_in_Microblogs">Koto and Rahmaningtyas, 2017</a>)
 and 2) <a href="https://github.com/annisanurulazhar/absa-playground/">hotel reviews</a>.
</span>

##### **Summarization**
<ul style="font-size:15px">
  <li>IndoSum, by <a href="https://arxiv.org/abs/1810.05334">Kurniawan and Louvan, (2018)</a>: is constructed from CNN Indonesian and Kumparan, with train/dev/test distribution: 14,262/750/3,762. </li>
  <li>Liputan6, by <a href="https://arxiv.org/abs/2011.00679">Koto et al., (2020)</a>: is the first large-scale Indonesian corpus for Abstractive and Extractive summarization. This data is from year 2000 - 2010. Train/Dev/Test distribution: 193,883/10,972/10,972.</li>
</ul>
- - - - - - - - - - - - - - - - - -  -
<span style="color:#233279; font-size:18px">&#9830; Discourse Coherence</span>

##### **Next Tweet Prediction**
<span style="font-size:15px">To evaluate model coherence, we design a next tweet prediction (NTP) 
task that is similar to the next sentence prediction (NSP) task used to train BERT
([Devlin et al., 2019](https://www.aclweb.org/anthology/N19-1423/)). In NTP, each instance consists of a Twitter thread 
(2–4 tweets) that we call the premise, and four possible options for the next tweet, one of which is the actual 
response from the original thread.</span>
<ul style="font-size:15px">
 <li> Train: 5,681 threads</li>
 <li> Development: 811 threads</li>
 <li> Test: 1,890 threads</li>
</ul>

##### **Tweet Ordering**
<span style="font-size:15px">This task is based on the sentence ordering task of 
[Barzilay and Lapata (2008)](https://www.aclweb.org/anthology/J08-1001/) to assess text relatedness. 
We construct the data by shuffling Twitter threads (containing 3–5 tweets), and assessing the predicted
ordering in terms of rank correlation (ρ) with the original.</span>
<ul style="font-size:15px">
 <li> Train: 4,327 threads</li>
 <li> Development: 760 threads</li>
 <li> Test: 1,521 threads</li>
</ul>


