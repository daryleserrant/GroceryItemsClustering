# GroceryItemsClustering

Clustering Grocery Items takehome challenge. From *A Collection of Data Science Takehome Challenges* by Guilio Palombo.  

## Challenge Description
Company XYZ is an online grocery store. In the current version of the website, they have manually grouped the items into a few categories based on their experience.

However, they now have a lot of data about user purchase history. Therefore, they would like to
put the data into use!

This is what they asked you to do:
* The company founder wants to meet with some of the best customers to go through a
focus group with them. You are asked to send the ID of the following customers to the
founder:
  - the customer who bought the most items overall in her lifetime  
  - for each item, the customer who bought that product the most
* Cluster items based on user co-purchase history. That is, create clusters of products that
have the highest probability of being bought together. The goal of this is to replace the
old/manually created categories with these new ones. Each item can belong to just one
cluster.

## Data
We have two tables:
* item_to_id - for each item, it gives the corresponding id. Columns:
  - **item_name**: the name of the item
  - **item_id**: the id of the item. Can be joined to the id in the other table.
* purchase_history - for each user purchase, the items bought. Columns:
  - **user_id**: the id of the user
  - **id**: comma-separated list of items brought together in that transaction
