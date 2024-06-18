import pandas as pd
from plotly.offline import  plot
import plotly.express as px
data = px.data.gapminder()


dataset=px.data.gapminder()
fig = px.scatter(dataset, x="gdpPercap", y="lifeExp", animation_frame="year",
                 animation_group="country",size="gdpPercap", color="continent",
                 hover_name="country",log_x=True, size_max=45,
                 range_x=[500,200000], range_y=[25,90],
                 labels=dict(gdpPercap="人均收入(PPP购买力标准)",lifeExp="人均寿命"))

plot(fig)

output_path = "C:/Users/17134/Desktop/gapminder_data.xlsx"
data.to_excel(output_path, index=False)
