

```python
%matplotlib inline
import pandas as pd
import cufflinks as cf
```


```python
import pandas_datareader as pdr
```


```python
fcx = pdr.DataReader('FCX', 'google')
```


```python
fcx.Close.iplot()
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/145.embed" height="525px" width="100%"></iframe>




```python
bumi = pdr.get_data_yahoo('BUMI.JK')
bumi.Close.iplot(title = 'BUMI')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/125.embed" height="525px" width="100%"></iframe>




```python
import plotly.tools as tls
tls.set_credentials_file(username='larry.pagi', api_key='BscI66DFJ3euOtn8ogG5')

```


```python
def f1(stock):
    df = pdr.get_data_yahoo(stock)
    return df.Close.iplot(title = stock)
```


```python
def mas_herry(stock):
    df = pdr.get_data_yahoo(stock)
    return df.Close.iplot(title = stock)
```


```python
f1('IBM')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/129.embed" height="525px" width="100%"></iframe>




```python
f1('BRMS.JK')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/131.embed" height="525px" width="100%"></iframe>




```python
f1('FCX')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/133.embed" height="525px" width="100%"></iframe>




```python
mas_herry('ELTY.JK')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/135.embed" height="525px" width="100%"></iframe>




```python
mas_herry('DEWA.JK')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/137.embed" height="525px" width="100%"></iframe>




```python
mas_herry('ENRG.JK')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/139.embed" height="525px" width="100%"></iframe>




```python
mas_herry('UNSP.JK')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/141.embed" height="525px" width="100%"></iframe>




```python
mas_herry('BNBR.JK')
```




<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~larry.pagi/143.embed" height="525px" width="100%"></iframe>




```python

```
