# Import necessary libraries
import pandas as pd
import plotly.graph_objects as go

# Example Data (replace with your actual data)
data = {'time': [1, 2, 3, 4, 5],
        'defect_rate': [0.05, 0.03, 0.08, 0.02, 0.06]}
df = pd.DataFrame(data)

# Create a line chart using Plotly
fig = go.Figure(data=go.Scatter(x=df['time'], y=df['defect_rate']))
fig.update_layout(title='Defect Rate over Time',
                  xaxis_title='Time (e.g., shifts)',
                  yaxis_title='Defect Rate')

# Show the chart (or save it to a file/web page)
fig.show()
