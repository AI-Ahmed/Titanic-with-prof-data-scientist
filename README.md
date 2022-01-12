# Titanic - Machine Learning from Disaster
---
Copyright [2021] [Data Scientist & ML Engineer: [Ahmed](https://www.kaggle.com/dsxavier/)]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

## An Overview

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

## [Data Dictionary](https://www.kaggle.com/c/titanic/data#:~:text=should%20look%20like.-,data%20dictionary,-Variable)

<table>
<thead>
  <tr>
    <th>Variable</th>
    <th>Definition</th>
    <th>Key</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>survival</td>
    <td>Survival</td>
    <td>0 = No, 1 = Yes</td>
  </tr>
  <tr>
    <td>pclass</td>
    <td>Ticket class</td>
    <td>1 = 1st, 2 = 2nd, 3 = 3rd</td>
  </tr>
  <tr>
    <td>sex</td>
    <td>Sex</td>
    <td></td>
  </tr>
  <tr>
    <td>Age</td>
    <td>Age in years</td>
    <td></td>
  </tr>
  <tr>
    <td>sibsp</td>
    <td># of siblings / spouses aboard the Titanic</td>
    <td></td>
  </tr>
  <tr>
    <td>parch</td>
    <td># of parents / children aboard the Titanic</td>
    <td></td>
  </tr>
  <tr>
    <td>ticket</td>
    <td>Ticket number</td>
    <td></td>
  </tr>
  <tr>
    <td>fare</td>
    <td>Passenger fare</td>
    <td></td>
  </tr>
  <tr>
    <td>cabin</td>
    <td>Cabin number</td>
    <td></td>
  </tr>
  <tr>
    <td>embarked</td>
    <td>Port of Embarkation</td>
    <td>C = Cherbourg, Q = Queenstown, S = Southampton</td>
  </tr>
</tbody>
</table>

---

## Table of Contents

<table>
<thead>
  <tr>
      <th><a href='#Table-of-Contents'>Table of Contents</a></th>
    <th></th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
      <td><a href='#Dependencies'>Dependencies</a><br></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#(A)-Import-Libraries'>(A) Import Libraries</a></td>
    <td></td>
  </tr>
  <tr>
      <td><a href='#Workflow-Pipeline'>Workflow Pipeline</a></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#1.-Data-Preprocessing'>1. Data Preprocessing</a></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
      <td><a href='#(A)-Data-Wrangling'>(A) Data Wrangling</a></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
      <td><a href='#(B)-Exploratory-Data-Analysis'>(B) Exploratory Data Analysis</a></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#2.-Train-&-Test-Split'>2. Train & Test Split</a></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#3.-Algorithm-Setup'>3. Algorithm Setup</a></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#4.-Model-Fitting'>4. Model Fitting</a></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#5.-Model-Predictions'>5. Model Predictions</a></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#6.-Model-Evalutaion'>6. Model Evalutaion</a></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
      <td><a href='#7.-Export-Predictions'>7. Export Predictions</a></td>
    <td></td>
  </tr>
</tbody>
</table>
