# Filter, Search and Sort
- These have to make sense to users
- They have to meet user expectations and match their "Mental Map" which is their model of how the world should work
- You need to understand the customer to implement these well

## Quick Wins / Lessons Learned
- **Make it obvious when we update lists of results**
   <br>(There have been several systems that updated so quickly that people thought they had done nothing. )
    <br>(In these instances it has been necessary to put a visual cue to make the user aware of the page having updated. )
  -   **Be Very Clear about how the Search , Sort or Filter works**



## Search
- Search can adhere to several logical models.  <br>It is usually Not Clear to users which one we are following BUT they will assume one of them anyway. 
- These Models at the highest level, include:
	- **Open Ended Single Word search** <br>
	  (The word is found somewhere in the contents Title, Text or Metadata)
	- **Open Ended Multi Word search**<br> 
	  (Any of the words are found in the contents Title, Text or Metadata
	- **Specific Phrase search** <br>
	  (The exact phrase is found somewhere in the contentsTitle, Text or Metadata)  
- They then can be subdivided into only looking for these words or phrases within: 
	- **Title** Only
	- **Text** Only
	- **Metadata** Only
	- Any combination of these
- They can also act as a: 
	- **Filter** <br>
	  *This is EXCLUSIVE* <br>
	  All results are shown until they are **EXCLUDED** by the search
	- **Search**  <br>
	  *This is ADDITIVE*  <br>
	  No results are shown untill they are **ADDED** by the search
- There are many other subtle variations but the most often encountered is: 
	- Some searches need every word in a phrase to be found 
	- Other searches need any single word from the phrase in order to return a result

All this detail is given to let you know just how many **Mental Models** users might have. 

!!! warning
    **When you are implementing a Search or Filter; It is critical that you make it clear to users how it works.**

## Sort
Sounds simple BUT:

- Sort options are often lost or reset when other options are selected (Filter etc...)
- Tell users when Sort Options are changed
- Make it even more obvious if it was not **Explicitly** done by them


## Search vs Filter
- It is often unclear if the text input to a Search Box will build up a list, or narrow down a list. 
	- **Filter** <br>
	  *This is **EXCLUSIVE*** <br>
	  All results are shown until they are **EXCLUDED** by the search
	- **Search**  <br>
	  *This is **ADDITIVE***  <br>
	  No results are shown until they are **ADDED** by the search



## Pagination
- People hate endless pages<br>BUT<br>they also hate excessive pagination
- Estimate the number of likely results and ensure that this fits onto 6 pages or less. 

!!! note "High Attention Listings"
    10-20 items per page are typical for content that requires more attention per item, like products in an e-commerce store or job listings.

!!! note "Low Attention Listings"
    20-50 items per page can be appropriate for lists that users might want to scan more quickly, like search results or entries in a directory.




## Trip Hazards
- **People have VERY STRONG opinions on what a Search Box should look like**
- **They also have strong views on WHERE it should be**
    - Make sure Search Box looks like a search box
    - Stick it at the top right of the page
- **People expect search to work the way they expect.** 
	- Be very clear if you are doing anything clever
	- State if the search is acting more like a filter.. 
- **Mixing Search and Filters is a minefield**
	- Users tend to hold a single mental model of how a thing works
	- When you mix in different models (Additive Search + Exclusive Filtering) it can get really confusing
	- If you are doing this: 
		- Tell users what you are doing
		- Make it obvious every time the results change

