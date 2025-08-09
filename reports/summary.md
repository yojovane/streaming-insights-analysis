# Streaming Insights — Summary

## Visuals

- content_type_boxplot.png -> C:\Users\Jovane\streaming-insights-analysis\images\content_type_boxplot.png
- hourly_engagement_heatmap.png -> C:\Users\Jovane\streaming-insights-analysis\images\hourly_engagement_heatmap.png
- clusters_sizes.png -> C:\Users\Jovane\streaming-insights-analysis\images\clusters_sizes.png

## Predictive Model (Linear Regression on completion_rate)

- Test R^2: 0.217
- Test MAE: 0.1321

### Top coefficients (absolute magnitude)

- device_type_mobile: -0.1004
- user_plan_free: -0.0951
- content_type_series: -0.0666
- user_plan_premium: 0.0398
- content_type_movie: -0.0255
- device_type_tablet: -0.0063
- device_type_tv: 0.0030
- duration_minutes: -0.0015
- start_hour: -0.0000
- couple_watching: 0.0000


## Couple-Watching Classifier (Logistic Regression)

- Test Accuracy: nan

## User Segmentation (KMeans k=4)

### Cluster counts
|   cluster |   count |
|----------:|--------:|
|         0 |    3936 |
|         1 |    3720 |
|         2 |    1220 |
|         3 |    2387 |

### Cluster means
|   cluster |   watched_minutes |   completion_rate |   couple_watching |
|----------:|------------------:|------------------:|------------------:|
|         0 |            26.631 |             0.737 |                 0 |
|         1 |            20.63  |             0.404 |                 0 |
|         2 |            80.757 |             0.744 |                 0 |
|         3 |            49.039 |             0.546 |                 0 |

