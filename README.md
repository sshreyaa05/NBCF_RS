### Predicting Missing Ratings and Recommending Items Using Neighborhood-Based Collaborative Filtering with Pearson Similarity
### Overview: 
This project focuses on predicting missing ratings and providing personalized recommendations using Neighborhood-Based Collaborative Filtering (CF) based on Pearson similarity. The dataset includes 5 users and 6 items, with some ratings missing. By leveraging both User-Based and Item-Based Collaborative Filtering, we aimed to predict the missing rating for User 3 on Item 6, and decide whether to recommend the item or not.

### Project Steps:

1. Data Preprocessing:
The dataset was preprocessed with standard scaling to normalize ratings, ensuring fair comparison between users and items.

2. Pearson Similarity:
Pearson correlation coefficient was used to measure the similarity between users (for UBCF) and items (for IBCF). This similarity metric calculates the degree of linear relationship between ratings, helping identify users or items that behave similarly.

3. User-Based Collaborative Filtering (UBCF):
Similarity between users was calculated using Pearson similarity, and User 3's rating for Item 6 was predicted based on ratings from similar users.

4. Item-Based Collaborative Filtering (IBCF):
Similarity between items was also determined using Pearson similarity, and User 3’s rating for Item 6 was predicted by considering ratings for items similar to Item 6.

5. Prediction and Recommendation Decision:
The predicted rating r_hat(3,6) for User 3 on Item 6 was calculated. If the predicted rating is considerable for recommendation, the item should be recommended to the user else not.

### Conclusion: 
By applying Pearson similarity in both User-Based and Item-Based Collaborative Filtering, we successfully predicted missing ratings and made personalized recommendations. Using User based approach the system do not recommend the item but using item based approach the system recommends the item 6 to user 3 based on its estimated rating.
