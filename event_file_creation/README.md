This is to create a synthetic events file (later stored within metarank/events/..) which will be used to train the XGBoost model

- **Kharif Rabi split events** :  The code is written such that the following interactions, users, items are created for random ranking events
  - Two kinds of users : 
    - Users with crop = 'kharif': They click on only items 1-5 
    - Users with crop = 'rabi' : They click on only items 6-10
  - Two kinds of items : 
    - Items 1-5: They have fertilizer = 'fertrilizer_1' and persticide in {'pesticide_2,pesticide_3}
    - Items 6-10: They have fertilizer in {'fertilizer_1,fertilizer_3'} and pesticide = pesticide_1
