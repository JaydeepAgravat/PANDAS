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
