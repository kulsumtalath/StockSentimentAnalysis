```python
import pandas as pd
```


```python
df=pd.read_csv('Data.csv', encoding = "ISO-8859-1")
```


```python
df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Date</th>
      <th>Label</th>
      <th>Top1</th>
      <th>Top2</th>
      <th>Top3</th>
      <th>Top4</th>
      <th>Top5</th>
      <th>Top6</th>
      <th>Top7</th>
      <th>Top8</th>
      <th>...</th>
      <th>Top16</th>
      <th>Top17</th>
      <th>Top18</th>
      <th>Top19</th>
      <th>Top20</th>
      <th>Top21</th>
      <th>Top22</th>
      <th>Top23</th>
      <th>Top24</th>
      <th>Top25</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2000-01-03</td>
      <td>0</td>
      <td>A 'hindrance to operations': extracts from the...</td>
      <td>Scorecard</td>
      <td>Hughes' instant hit buoys Blues</td>
      <td>Jack gets his skates on at ice-cold Alex</td>
      <td>Chaos as Maracana builds up for United</td>
      <td>Depleted Leicester prevail as Elliott spoils E...</td>
      <td>Hungry Spurs sense rich pickings</td>
      <td>Gunners so wide of an easy target</td>
      <td>...</td>
      <td>Flintoff injury piles on woe for England</td>
      <td>Hunters threaten Jospin with new battle of the...</td>
      <td>Kohl's successor drawn into scandal</td>
      <td>The difference between men and women</td>
      <td>Sara Denver, nurse turned solicitor</td>
      <td>Diana's landmine crusade put Tories in a panic</td>
      <td>Yeltsin's resignation caught opposition flat-f...</td>
      <td>Russian roulette</td>
      <td>Sold out</td>
      <td>Recovering a title</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2000-01-04</td>
      <td>0</td>
      <td>Scorecard</td>
      <td>The best lake scene</td>
      <td>Leader: German sleaze inquiry</td>
      <td>Cheerio, boyo</td>
      <td>The main recommendations</td>
      <td>Has Cubie killed fees?</td>
      <td>Has Cubie killed fees?</td>
      <td>Has Cubie killed fees?</td>
      <td>...</td>
      <td>On the critical list</td>
      <td>The timing of their lives</td>
      <td>Dear doctor</td>
      <td>Irish court halts IRA man's extradition to Nor...</td>
      <td>Burundi peace initiative fades after rebels re...</td>
      <td>PE points the way forward to the ECB</td>
      <td>Campaigners keep up pressure on Nazi war crime...</td>
      <td>Jane Ratcliffe</td>
      <td>Yet more things you wouldn't know without the ...</td>
      <td>Millennium bug fails to bite</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2000-01-05</td>
      <td>0</td>
      <td>Coventry caught on counter by Flo</td>
      <td>United's rivals on the road to Rio</td>
      <td>Thatcher issues defence before trial by video</td>
      <td>Police help Smith lay down the law at Everton</td>
      <td>Tale of Trautmann bears two more retellings</td>
      <td>England on the rack</td>
      <td>Pakistan retaliate with call for video of Walsh</td>
      <td>Cullinan continues his Cape monopoly</td>
      <td>...</td>
      <td>South Melbourne (Australia)</td>
      <td>Necaxa (Mexico)</td>
      <td>Real Madrid (Spain)</td>
      <td>Raja Casablanca (Morocco)</td>
      <td>Corinthians (Brazil)</td>
      <td>Tony's pet project</td>
      <td>Al Nassr (Saudi Arabia)</td>
      <td>Ideal Holmes show</td>
      <td>Pinochet leaves hospital after tests</td>
      <td>Useful links</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2000-01-06</td>
      <td>1</td>
      <td>Pilgrim knows how to progress</td>
      <td>Thatcher facing ban</td>
      <td>McIlroy calls for Irish fighting spirit</td>
      <td>Leicester bin stadium blueprint</td>
      <td>United braced for Mexican wave</td>
      <td>Auntie back in fashion, even if the dress look...</td>
      <td>Shoaib appeal goes to the top</td>
      <td>Hussain hurt by 'shambles' but lays blame on e...</td>
      <td>...</td>
      <td>Putin admits Yeltsin quit to give him a head s...</td>
      <td>BBC worst hit as digital TV begins to bite</td>
      <td>How much can you pay for...</td>
      <td>Christmas glitches</td>
      <td>Upending a table, Chopping a line and Scoring ...</td>
      <td>Scientific evidence 'unreliable', defence claims</td>
      <td>Fusco wins judicial review in extradition case</td>
      <td>Rebels thwart Russian advance</td>
      <td>Blair orders shake-up of failing NHS</td>
      <td>Lessons of law's hard heart</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2000-01-07</td>
      <td>1</td>
      <td>Hitches and Horlocks</td>
      <td>Beckham off but United survive</td>
      <td>Breast cancer screening</td>
      <td>Alan Parker</td>
      <td>Guardian readers: are you all whingers?</td>
      <td>Hollywood Beyond</td>
      <td>Ashes and diamonds</td>
      <td>Whingers - a formidable minority</td>
      <td>...</td>
      <td>Most everywhere:  UDIs</td>
      <td>Most wanted:  Chloe lunettes</td>
      <td>Return of the cane 'completely off the agenda'</td>
      <td>From Sleepy Hollow to Greeneland</td>
      <td>Blunkett outlines vision for over 11s</td>
      <td>Embattled Dobson attacks 'play now, pay later'...</td>
      <td>Doom and the Dome</td>
      <td>What is the north-south divide?</td>
      <td>Aitken released from jail</td>
      <td>Gone aloft</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 27 columns</p>
</div>




```python
train = df[df['Date'] < '20150101']
test = df[df['Date'] > '20141231']
```


```python
# Removing punctuations
data=train.iloc[:,2:27]
data.replace("[^a-zA-Z]"," ",regex=True, inplace=True)

# Renaming column names for ease of access
list1= [i for i in range(25)]
new_Index=[str(i) for i in list1]
data.columns= new_Index
data.head(5)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
      <th>5</th>
      <th>6</th>
      <th>7</th>
      <th>8</th>
      <th>9</th>
      <th>...</th>
      <th>15</th>
      <th>16</th>
      <th>17</th>
      <th>18</th>
      <th>19</th>
      <th>20</th>
      <th>21</th>
      <th>22</th>
      <th>23</th>
      <th>24</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>A  hindrance to operations   extracts from the...</td>
      <td>Scorecard</td>
      <td>Hughes  instant hit buoys Blues</td>
      <td>Jack gets his skates on at ice cold Alex</td>
      <td>Chaos as Maracana builds up for United</td>
      <td>Depleted Leicester prevail as Elliott spoils E...</td>
      <td>Hungry Spurs sense rich pickings</td>
      <td>Gunners so wide of an easy target</td>
      <td>Derby raise a glass to Strupar s debut double</td>
      <td>Southgate strikes  Leeds pay the penalty</td>
      <td>...</td>
      <td>Flintoff injury piles on woe for England</td>
      <td>Hunters threaten Jospin with new battle of the...</td>
      <td>Kohl s successor drawn into scandal</td>
      <td>The difference between men and women</td>
      <td>Sara Denver  nurse turned solicitor</td>
      <td>Diana s landmine crusade put Tories in a panic</td>
      <td>Yeltsin s resignation caught opposition flat f...</td>
      <td>Russian roulette</td>
      <td>Sold out</td>
      <td>Recovering a title</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Scorecard</td>
      <td>The best lake scene</td>
      <td>Leader  German sleaze inquiry</td>
      <td>Cheerio  boyo</td>
      <td>The main recommendations</td>
      <td>Has Cubie killed fees</td>
      <td>Has Cubie killed fees</td>
      <td>Has Cubie killed fees</td>
      <td>Hopkins  furious  at Foster s lack of Hannibal...</td>
      <td>Has Cubie killed fees</td>
      <td>...</td>
      <td>On the critical list</td>
      <td>The timing of their lives</td>
      <td>Dear doctor</td>
      <td>Irish court halts IRA man s extradition to Nor...</td>
      <td>Burundi peace initiative fades after rebels re...</td>
      <td>PE points the way forward to the ECB</td>
      <td>Campaigners keep up pressure on Nazi war crime...</td>
      <td>Jane Ratcliffe</td>
      <td>Yet more things you wouldn t know without the ...</td>
      <td>Millennium bug fails to bite</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Coventry caught on counter by Flo</td>
      <td>United s rivals on the road to Rio</td>
      <td>Thatcher issues defence before trial by video</td>
      <td>Police help Smith lay down the law at Everton</td>
      <td>Tale of Trautmann bears two more retellings</td>
      <td>England on the rack</td>
      <td>Pakistan retaliate with call for video of Walsh</td>
      <td>Cullinan continues his Cape monopoly</td>
      <td>McGrath puts India out of their misery</td>
      <td>Blair Witch bandwagon rolls on</td>
      <td>...</td>
      <td>South Melbourne  Australia</td>
      <td>Necaxa  Mexico</td>
      <td>Real Madrid  Spain</td>
      <td>Raja Casablanca  Morocco</td>
      <td>Corinthians  Brazil</td>
      <td>Tony s pet project</td>
      <td>Al Nassr  Saudi Arabia</td>
      <td>Ideal Holmes show</td>
      <td>Pinochet leaves hospital after tests</td>
      <td>Useful links</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Pilgrim knows how to progress</td>
      <td>Thatcher facing ban</td>
      <td>McIlroy calls for Irish fighting spirit</td>
      <td>Leicester bin stadium blueprint</td>
      <td>United braced for Mexican wave</td>
      <td>Auntie back in fashion  even if the dress look...</td>
      <td>Shoaib appeal goes to the top</td>
      <td>Hussain hurt by  shambles  but lays blame on e...</td>
      <td>England s decade of disasters</td>
      <td>Revenge is sweet for jubilant Cronje</td>
      <td>...</td>
      <td>Putin admits Yeltsin quit to give him a head s...</td>
      <td>BBC worst hit as digital TV begins to bite</td>
      <td>How much can you pay for</td>
      <td>Christmas glitches</td>
      <td>Upending a table  Chopping a line and Scoring ...</td>
      <td>Scientific evidence  unreliable   defence claims</td>
      <td>Fusco wins judicial review in extradition case</td>
      <td>Rebels thwart Russian advance</td>
      <td>Blair orders shake up of failing NHS</td>
      <td>Lessons of law s hard heart</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Hitches and Horlocks</td>
      <td>Beckham off but United survive</td>
      <td>Breast cancer screening</td>
      <td>Alan Parker</td>
      <td>Guardian readers  are you all whingers</td>
      <td>Hollywood Beyond</td>
      <td>Ashes and diamonds</td>
      <td>Whingers   a formidable minority</td>
      <td>Alan Parker   part two</td>
      <td>Thuggery  Toxins and Ties</td>
      <td>...</td>
      <td>Most everywhere   UDIs</td>
      <td>Most wanted   Chloe lunettes</td>
      <td>Return of the cane  completely off the agenda</td>
      <td>From Sleepy Hollow to Greeneland</td>
      <td>Blunkett outlines vision for over   s</td>
      <td>Embattled Dobson attacks  play now  pay later ...</td>
      <td>Doom and the Dome</td>
      <td>What is the north south divide</td>
      <td>Aitken released from jail</td>
      <td>Gone aloft</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 25 columns</p>
</div>




```python
#converting headlines to lower case
for index in new_Index:
    data[index]=data[index].str.lower()
data.head(1)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
      <th>5</th>
      <th>6</th>
      <th>7</th>
      <th>8</th>
      <th>9</th>
      <th>...</th>
      <th>15</th>
      <th>16</th>
      <th>17</th>
      <th>18</th>
      <th>19</th>
      <th>20</th>
      <th>21</th>
      <th>22</th>
      <th>23</th>
      <th>24</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>a  hindrance to operations   extracts from the...</td>
      <td>scorecard</td>
      <td>hughes  instant hit buoys blues</td>
      <td>jack gets his skates on at ice cold alex</td>
      <td>chaos as maracana builds up for united</td>
      <td>depleted leicester prevail as elliott spoils e...</td>
      <td>hungry spurs sense rich pickings</td>
      <td>gunners so wide of an easy target</td>
      <td>derby raise a glass to strupar s debut double</td>
      <td>southgate strikes  leeds pay the penalty</td>
      <td>...</td>
      <td>flintoff injury piles on woe for england</td>
      <td>hunters threaten jospin with new battle of the...</td>
      <td>kohl s successor drawn into scandal</td>
      <td>the difference between men and women</td>
      <td>sara denver  nurse turned solicitor</td>
      <td>diana s landmine crusade put tories in a panic</td>
      <td>yeltsin s resignation caught opposition flat f...</td>
      <td>russian roulette</td>
      <td>sold out</td>
      <td>recovering a title</td>
    </tr>
  </tbody>
</table>
<p>1 rows × 25 columns</p>
</div>




```python
' '.join(str(x) for x in data.iloc[1,0:25])
#text preprocessing=combining all the 25 headlines into one paragraph
```




    'scorecard the best lake scene leader  german sleaze inquiry cheerio  boyo the main recommendations has cubie killed fees  has cubie killed fees  has cubie killed fees  hopkins  furious  at foster s lack of hannibal appetite has cubie killed fees  a tale of two tails i say what i like and i like what i say elbows  eyes and nipples task force to assess risk of asteroid collision how i found myself at last on the critical list the timing of their lives dear doctor irish court halts ira man s extradition to northern ireland burundi peace initiative fades after rebels reject mandela as mediator pe points the way forward to the ecb campaigners keep up pressure on nazi war crimes suspect jane ratcliffe yet more things you wouldn t know without the movies millennium bug fails to bite'




```python
headlines = []
for row in range(0,len(data.index)):
    headlines.append(' '.join(str(x) for x in data.iloc[row,0:25]))
```


```python
headlines[245]
```




    'nasty nick puts heat on pope in today poll bbc  to cram news into one minute paraglider arrested at buckingham palace mps urge delaying reading and writing woodhead  once a tory  always a tory bin laden link to frankfurt terror suspects britain gets extended white christmas tv ads prompt rush to join police three sought for racist attack on turk explosions rock israel after summit cancelled early bird bargain hunters brave the freeze tel aviv blast hits slender peace hopes alarm as drug company chief joins watchdog billions lost in contracts failure mutiny threat over health councils tube cashes in on movie magic europe s centre cannot hold obituary  stephen mitchell peckham strives to discover a new image poster s lesbian embrace breaks advertising taboo bush adviser talks tough on colombia shell cuts price of unleaded by  p a litre top judge attacks prison  cancer  middle east talks founder dissenters'




```python
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.ensemble import RandomForestClassifier
```


```python
#implement bag of words
countvector=CountVectorizer(ngram_range=(2,2))
#ngram takes a word and converts them to vectors
traindataset=countvector.fit_transform(headlines)

```


```python
traindataset[0]
```




    <1x584289 sparse matrix of type '<class 'numpy.int64'>'
    	with 138 stored elements in Compressed Sparse Row format>




```python
#implement RandomForest Classifer
randomclassifier=RandomForestClassifier(n_estimators=200,criterion='entropy')
randomclassifier.fit(traindataset,train['Label'])
```




    RandomForestClassifier(criterion='entropy', n_estimators=200)




```python
#predict for test dataset #do the same steps for test dataset
test_transform= []
for row in range(0,len(test.index)):
    test_transform.append(' '.join(str(x) for x in test.iloc[row,2:27]))
test_dataset = countvector.transform(test_transform)
predictions = randomclassifier.predict(test_dataset)
    
```


```python
#import lib to check accuracy
from sklearn.metrics import classification_report,confusion_matrix,accuracy_score
```


```python
matrix=confusion_matrix(test['Label'],predictions)
print(matrix)
score=accuracy_score(test['Label'],predictions)
print(score)
report=classification_report(test['Label'],predictions)
print(report)
```

    [[138  48]
     [  5 187]]
    0.8597883597883598
                  precision    recall  f1-score   support
    
               0       0.97      0.74      0.84       186
               1       0.80      0.97      0.88       192
    
        accuracy                           0.86       378
       macro avg       0.88      0.86      0.86       378
    weighted avg       0.88      0.86      0.86       378
    
    


```python

```
