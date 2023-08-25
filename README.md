# PANDAS

## 1. Series

- Pandas Series
- Series from lists
- Series from dict
- Series Attributes
- Series using read_csv
- Series methods
- Series Maths Methods
- Series Indexing
- Series with Python Functionalities
- Boolean Indexing on Series
- Plotting Graphs on Series
- Some Important Series Methods

## 2. DataFrame

- Pandas DataFrame
- Creating DataFrame
- DataFrame Attributes and Methods
- Math Methods
- Selecting cols from a DataFrame
- Selecting rows from a DataFrame
- Selecting both rows and cols
- Filtering a DataFrame
- Adding new cols

```python
ds = pd.Series(data=,index=,name=)
ds = pd.read_csv(,index_col=)
ds.size
ds.count()
ds.dtype
ds.name
ds.is_unique
ds.index
ds.values

ds.head()
ds.tail()
ds.sample()
ds.sum() 
ds.min()
ds.max()
ds.mean()
ds.median()
ds.mode()
ds.std()
ds.var()

ds.value_counts()
ds.sort_values(ascending=False)
ds.sort_index(ascending=False)
ds.describe()
ds.isnull()

ds.iloc[]
ds.iat[]
ds.loc[]
ds.at[]

ds.fillna()
ds.dropna()

ds.isin() 
ds.between()
ds.clip()

ds.duplicated()
ds.drop_duplicates(keep='last')

ds.plot()
ds.apply()
ds.copy()
sys.getsizeof(ds)
```

```python
df = pd.DataFrame(data=,columns=[])
df = pd.read_csv('')
df.rename(columns={'old':'new','old1':'new1'},inplace=True)
df.set_index('iname',inplace=True)

df.shape
df.dtypes
df.index
df.columns
df.values

df.head()
df.tail()
df.sample()
df.info()
df.describe()

df.isnull().sum()
df.duplicated.sum()

df.sum(axis=0)
df.mean(axis=1)
df.var()

df['col']
df[['c1','c2','c3']]
df.iloc[]
df.loc[]

df['newc'] = 'val'

df.dropna(inplace=True)
```
