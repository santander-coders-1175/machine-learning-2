## Churn Predictor Model

### About

This project, developed by Juan Vieira and Mille Amorim, is about building a classifier model to deal with the task of predicting which subscribers to a music streaming platform will stop subscribing to the service (churn). 

### Goals

Our aim will be to cluster the music streaming platform's subscriber base and use other statistical approaches to build a model capable of predicting churn, in order to help the business area in its retention strategies.

**Churn scenario**

Churn is generally the event that a customer stops using a service.

It is an unbalanced classification problem, where the (positive) churn cases are usually a small fraction of the total.
Erring in predicting a churn can be more costly than generating a false positive, as it is more important to identify those with a high probability of churn for preventive action.

As explained above, we must avoid the loss of False Negatives, so the target metric will be a recall above 80%.

### Data Description

```
RangeIndex: 125000 entries, 0 to 124999
Data columns (total 20 columns):
 #   Column                      Non-Null Count   Dtype  
---  ------                      --------------   -----  
 0   customer_id                 125000 non-null  int64  
 1   age                         125000 non-null  float64
 2   location                    125000 non-null  object 
 3   subscription_type           125000 non-null  object 
 4   payment_plan                125000 non-null  object 
 5   num_subscription_pauses     125000 non-null  int64  
 6   payment_method              125000 non-null  object 
 7   customer_service_inquiries  125000 non-null  object 
 8   signup_date                 125000 non-null  int64  
 9   weekly_hours                125000 non-null  float64
 10  average_session_length      125000 non-null  float64
 11  song_skip_rate              125000 non-null  float64
 12  weekly_songs_played         125000 non-null  int64  
 13  weekly_unique_songs         125000 non-null  int64  
 14  num_favorite_artists        125000 non-null  int64  
 15  num_platform_friends        125000 non-null  int64  
 16  num_playlists_created       125000 non-null  int64  
 17  num_shared_playlists        125000 non-null  int64  
 18  notifications_clicked       125000 non-null  int64  
 19  churned                     125000 non-null  int64  
dtypes: float64(4), int64(11), object(5)
memory usage: 19.1+ MB
```

Authors: Mille Amorim, Juan Vieira
