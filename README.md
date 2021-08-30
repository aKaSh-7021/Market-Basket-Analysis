# <p align=center> Market-Basket-Analysis

## Abstract

<p align=justify>
All of us must have done e-shopping, right? We go to the website to buy a specific item but eventually end up with a lot more other stuffs in our cart at the checkout, right? But how do the retailers manage to tempt us into buying stuffs that we do not actually intend to buy in the first place?</p>
<p align=justify>
We live in the era of e-commerce and digital marketing. We have even small scale businesses going online as the opportunities are endless. Since a huge chunk of the people who have access to internet is switching to online shopping, large retailers are actively searching for ways to increase their profit. Market Basket analysis is one such key techniques used by large retailers to to increase sales by understanding the customers' purchasing behaviour & patterns.</p>
<p align=justify> 
Let's look into the functionality with an example. Customers who buy bread are more likely to buy jam as well, similarly people who buy laptops are likely to buy laptop bags as well. So placing these set of items together correctly will increase the chance of the purchase of the second item is effectively. Now lets say we find out that people who buy bread buy jam most of the time, how can we make them buy a third item say eggs? what if we place an offer that they can't deny? Lets give them a discount of 30% on eggs, they will be tempted to buy the eggs right?</p>
<p align=justify>
This is how the market basket analysis work, we find relationships between items that go together within the business context. For the purposes of customer centricity, market basket analysis examines collections of items to identify affinities that are relevant within the different contexts of the customer touch points such as:</p>

  - <p align=justify><b>Product Placement</b>: Identifying products that may often be purchased together and arranging the placement of those items close by to encourage the purchaser to buy both items.
  - <p align=justify><b>Point-of-Sale</b>: Companies may use the affinity grouping of multiple products as an indication that customers may be predisposed to buying certain sets of products at the same time. This enables the presentation of items for cross-selling, or may suggest that customers may be willing to buy more items when certain products are bundled together.
- <p align=justify><b>Customer Retention</b>: When customers contact a business to sever a relationship, a company representative may use market basket analysis to determine the right incentives to offer in order to retain the customer’s business.

  
## Problem Statement
<p align=justify>To determine the association between various products in the basket by analysing the customer purchase pattern of multiple items. The idea is to find answers to the following questions:</p>

- What are the most frequently sold items? 
- What are the consequents of the chosen items?
- How confident are the consequents of antecedents?
- What are the most important items that should always be in the store?
- How the frequent itemset network looks like?

  
## Methodologies 🔰
<details>
<summary><b>Association Rule Mining</b></summary>
<p align=justify>
Association rule mining is a data mining approach used to explore and interpret large transactional datasets to identify unique patterns and rules. Association rules identify frequent patterns and associations among every distinct set of transactions. This is generally carried out in two steps:

- Itemset Generation
- Rule Generation
</p>
</details>
  
<details>
<summary><b>ML Algorithms</b></summary>
<p align=justify>

1. **Apriori Algorithm :** It allows us to generate all frequent itemsets by pruning all the supersets of an itemset which do not satisfy the minimum support threshold. It works on the basis of the Apriori principle which states that <em>"every subset of a frequent itemset must also be frequent"</em>.
  
  - generates all itemsets of length one & prune itemsets that do not satisfy the minimumn threshold creteria
  - generates all itemsets of length two & prune itemsets that do not satisfy the minimumn threshold creteria
  - continues the process with a unit increase in the length of itemsets at every iteration until the maximal frequent itemset is achieved
  </p>
- <p align=justify><b>ECLAT Algorithm :</b> It is a depth-first search based algorithm which uses vertical data format which makes it more memory efficient and faster than the Apriori algorithm as it does not have to scan the entire database repeatedly.
  
  - stores for each item the transaction ids in a vertical dat format
  - determine the support of k-item sets by intersecting the list of transaction ids of two (k-1)-item sets from which it is generated
  </p>
  
</details>  
<details>
<summary><b>Evaluation Metrices</b></summary>
<p align=justify>The frequent itemsets and association rules are generated generally on the basis of three evaluation metrices i.e support, confidence and lift. Let X be an antecedent and Y be the corresponding consequent. Then,
  
  - `Support(X) = probability(X)`
  - `Confidence(X → Y) = support(X,Y)/support(X)`
  - `Lift(X → Y) = support(X,Y)/[support(X).support(Y)]`
</p>
</details>
  
## Approach
- Importing Necessary Dependencies
- Loading and Reading the Datasets
- Data Exploration and Visualization
- Data Preprocessing
  - Data Cleaning
  - Transforming data to one transaction per row
  - One Hot Encoding of purchases made
- Generating Association Rules
- Refining the Rules


  
  
> ## Featured Notebooks/Analysis/Deliverables
<details>
           <summary>NoteBook 1</summary>
           <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
         </details>
 
## Conclusion

<div class="intercom-reaction-picker" align="center" dir="ltr">
    <div class="intercom-reaction-prompt">Did this answer your question?</div>
      <button class="intercom-reaction" data-reaction-text="disappointed" tabindex="0" aria-label="Disappointed Reaction">
        <span data-emoji="disappointed" title="Disappointed" align="center">😞</span>
      </button>
      <button class="intercom-reaction" data-reaction-text="neutral_face" tabindex="0" aria-label="Neutral face Reaction">
        <span data-emoji="neutral_face" title="Neutral face">😐</span>
      </button>
      <button class="intercom-reaction" data-reaction-text="smiley" tabindex="0" aria-label="Smiley Reaction">
        <span data-emoji="smiley" title="Smiley">😃</span>
      </button>
  </div>
