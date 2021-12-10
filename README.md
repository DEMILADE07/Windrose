# Windrose
A data visualization plot showing the strength, frequency, and direction of wind pressure


import plotly.express as px
df = px.data.wind()
fig = px.bar_polar(df, r='frequency', theta='direction',
                   color='strength', template='plotly_dark',
                   color_discrete_sequence= px.colors.sequential.Plasma_r)
fig.show()
