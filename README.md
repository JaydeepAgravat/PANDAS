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

## 3. Methods

- Series methods
- DataFrame methods

## 4. Groupby

- groupby
- Applying builtin aggregation method on groupby objects
- GroupBy Attributes and Methods
- Aggregation method: dict & list
- Looping on groups
- apply
- groupby on multiple cols
- agg on multiple groupby

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
```python
# Series

ds.astype(dtype=)
ds.value_counts()
ds.sort_values(ascending=)
ds.rank(ascending=)
ds.sort_index(ascending=)
ds.reset_index(inplace=)
ds.unique()
ds.nunique()
ds.isnull()
ds.notnull()
ds.hasnans
ds.dropna(how='any')
ds.fillna(value=, method='bfill', inplace=)
ds.drop_duplicates(keep='first')
ds.drop(index=[], inplace=)
ds.apply(func)
ds.isin(values=[])
ds.corr(other=)
ds.nlargest(n=5, keep='last')
ds.nsmallest(n=5)

# DataFrame
df.value_counts()
df.sort_values(['ds1','ds2'], ascending=[True, False], na_position='first', inplace=)
df.sort_index(ascending=)
df.set_index('ds', inplace=)
df.reset_index(inplace=)
df.rename(columns={"oldc":"newc"}, inplace=)
df.rename(index={"oldv":"newv"}, inplace=)
df.isnull()
df.notnull()
df.dropna(subset=[], how='all')
df.fillna()
df.drop_duplicates(subset=[], keep='last')
df.drop(index=[], columns=[], inplace=)
df.drop(labels=[], axis=1, inplace=)
df.apply(func=, axis=)
df.isin(values=[])
df.corr(numeric_only=True)
df.nlargest(n=5, columns=[], keep='first')
df.nsmallest(n=5, columns=[], keep='all')
df.insert(loc=, columns, value=ds)
```

```python
gbo.groups
len(gbo)
gbo.size()
gbo.max()
gbo.count()
gbo.describe()
dbo.sample()
gbo.first()
gbo.last()
gbo.nth()
gbo.get_group()
gbo.nunique()
gbo.agg({})
gbo.agg([])
gbo.apply()
for _,data in gbo:
  pass
```
