# plotly

promemoria per integrazione plotly in flask

## esempio

```python
import plotly.express as px
gapminder_df = px.data.gapminder()
#gapminder_df

px.scatter(data_frame=gapminder_df,
          x='gdpPercap',
          y='lifeExp',
          size='pop',
          color='continent',
          title='Life Span',
          labels={'gdpPercap': 'Wealth',
                 'lifeExp': 'Life Span'},
          log_x=True,
          range_y=[25,95],
          hover_name='country',
          animation_frame='year',
          height=600,size_max=100)
          
```          
