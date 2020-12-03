---
layout: page
title: Leaderboard
permalink: /leaderboard/
icon: th-list
type: page
---
* content
{:toc}

<style>
.styled-table {
    border-collapse: collapse;
    margin: 20px 0;
    font-size: 0.9em;
    font-family: sans-serif;
    min-width: 400px;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
}
.styled-table thead tr {
    background-color: #009879;
    color: #ffffff;
    text-align: left;
}
.styled-table th,
.styled-table td {
    padding: 7px 5px;
}
.styled-table tbody tr {
    border-bottom: 1px solid #dddddd;
}

.styled-table tbody tr:nth-of-type(even) {
    background-color: #f3f3f3;
}

.styled-table tbody tr:last-of-type {
    border-bottom: 2px solid #009879;
}
.styled-table tbody tr.active-row {
    font-weight: bold;
    color: #009879;
}
</style>

<span style="font-size:16px">We open any submission for each category listed below. Please follow 
<a href="https://github.com/indolem/indolem" target="_blank">this instruction</a> &#128522; &#128522; &#128522; &#128522; &#128522;</span>

- - - - - - - - - - - - -

##### **POS and NER**

<table class="styled-table">
    <thead>
        <tr>
            <th>Method</th>
            <th style="text-align:center">POS (Acc)</th>
            <th style="text-align:center">NER-UGM (F1)</th>
            <th style="text-align:center">NER-UI (F1)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>IndoBERT (Koto et al., 2020)</td>
            <td style="text-align:center">96.8</td>
            <td style="text-align:center">74.9</td>
            <td style="text-align:center">90.1</td>
        </tr>
        <tr>
            <td>MalayBERT</td>
            <td style="text-align:center">96.8</td>
            <td style="text-align:center">73.2</td>
            <td style="text-align:center">87.4</td>
        </tr>
        <tr>
            <td>mBERT</td>
            <td style="text-align:center">96.8</td>
            <td style="text-align:center">71.6</td>
            <td style="text-align:center">82.2</td>
        </tr>
        <tr>
            <td>BiLSTM (Lample et al., 2016)</td>
            <td style="text-align:center">95.4</td>
            <td style="text-align:center">70.9</td>
            <td style="text-align:center">82.2</td>
        </tr>
    </tbody>
</table>
- - - - - - - - - - - - -

##### **Dependency Parsing**

<table class="styled-table">
    <thead>
        <tr>
            <th rowspan="2">Method</th>
            <th colspan="2" style="text-align:center">Indo-GSD</th>
            <th colspan="2" style="text-align:center">Indo-PUD</th>
        </tr>
        <tr>
            <th style="text-align:center">UAS</th>
            <th style="text-align:center">LAS</th>
            <th style="text-align:center">UAS</th>
            <th style="text-align:center">LAS</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>IndoBERT (Koto et al., 2020)</td>
            <td style="text-align:center">87.1</td>
            <td style="text-align:center">82.3</td>
            <td style="text-align:center">89.2</td>
            <td style="text-align:center">83.9</td>
        </tr>
        <tr>
            <td>MalayBERT</td>
            <td style="text-align:center">86.9</td>
            <td style="text-align:center">81.8</td>
            <td style="text-align:center">88.9</td>
            <td style="text-align:center">83.6</td>
        </tr>
        <tr>
            <td>mBERT</td>
            <td style="text-align:center">86.9</td>
            <td style="text-align:center">81.8</td>
            <td style="text-align:center">90.6</td>
            <td style="text-align:center">85.4</td>
        </tr>
        <tr>
            <td>Kondratyuk and Straka (2019)</td>
            <td style="text-align:center">86.5</td>
            <td style="text-align:center">80.1</td>
            <td style="text-align:center">77.5</td>
            <td style="text-align:center">56.9</td>
        </tr>
    </tbody>
</table>
- - - - - - - - - - - - -

##### **Semantic**

<table class="styled-table">
    <thead>
        <tr>
            <th rowspan="2">Method</th>
            <th colspan="1" style="text-align:center">Sentiment</th>
            <th colspan="3" style="text-align:center">IndoSum</th>
            <th colspan="3" style="text-align:center">Liputan6 (Sum)</th>
        </tr>
        <tr>
            <th style="text-align:center">F1</th>
            <th style="text-align:center">R1</th>
            <th style="text-align:center">R2</th>
            <th style="text-align:center">RL</th>
            <th style="text-align:center">R1</th>
            <th style="text-align:center">R2</th>
            <th style="text-align:center">RL</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>IndoBERT (Koto et al., 2020)</td>
            <td style="text-align:center">84.1</td>
            <td style="text-align:center">69.9</td>
            <td style="text-align:center">62.9</td>
            <td style="text-align:center">69.2</td>
            <td style="text-align:center">41.1</td>
            <td style="text-align:center">22.9</td>
            <td style="text-align:center">38.9</td>
        </tr>
        <tr>
            <td>MalayBERT</td>
            <td style="text-align:center">82.0</td>
            <td style="text-align:center">68.4</td>
            <td style="text-align:center">61.4</td>
            <td style="text-align:center">67.7</td>
            <td style="text-align:center">--</td>
            <td style="text-align:center">--</td>
            <td style="text-align:center">--</td>
        </tr>
        <tr>
            <td>mBERT</td>
            <td style="text-align:center">76.6</td>
            <td style="text-align:center">68.4</td>
            <td style="text-align:center">61.7</td>
            <td style="text-align:center">47.8</td>
            <td style="text-align:center">39.8</td>
            <td style="text-align:center">21.8</td>
            <td style="text-align:center">37.0</td>
        </tr>
        <tr>
            <td>BiLSTM</td>
            <td style="text-align:center">71.6</td>
            <td style="text-align:center">67.9</td>
            <td style="text-align:center">61.7</td>
            <td style="text-align:center">67.2</td>
            <td style="text-align:center">36.1</td>
            <td style="text-align:center">19.2</td>
            <td style="text-align:center">33.6</td>
        </tr>
    </tbody>
</table>
- - - - - - - - - - - - -

##### **Discourse Coherency**

<table class="styled-table">
    <thead>
        <tr>
            <th rowspan="1">Method</th>
            <th colspan="1" style="text-align:center">NTP (Acc)</th>
            <th colspan="1" style="text-align:center">Tweet Ordering (&rho;)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>IndoBERT (Koto et al., 2020)</td>
            <td style="text-align:center">93.7</td>
            <td style="text-align:center">0.59</td>
        </tr>
        <tr>
            <td>MalayBERT</td>
            <td style="text-align:center">93.1</td>
            <td style="text-align:center">0.51</td>
        </tr>
        <tr>
            <td>mBERT</td>
            <td style="text-align:center">92.4</td>
            <td style="text-align:center">0.53</td>
        </tr>
        <tr>
            <td>BiLSTM</td>
            <td style="text-align:center">73.6</td>
            <td style="text-align:center">0.45</td>
        </tr>
    </tbody>
</table>

