***
- [f] Listing and pagination (query params, fields filtering, pagination)

- [b] Link: https://www.atatus.com/blog/rest-api-design-filtering-sorting-and-pagination/

- [i] Filtering:
- [I] Filtering methods:  Path parameters, Query parameters, Request body
- Comparison and conjunction operators in filtering:
	*Equal to (=), Not equal to (!=), Less than (<), Less than or equal to (<=), Greater than (>), Greater than or equal to (>=)*

- [i] Pagination: 
      Offset Pagination, Cursor-based Pagination, Keyset Pagination, Seek Pagination
   
- *Offset Pagination:*
	- [b] Link: https://api.example.com/products?limit=10&offset=20

	Offset pagination is a widely used method in RESTful APIs that facilitates the return of a selected subset of data from a larger collection. With this technique, developers can specify an offset value and a limit value, which enable them to determine which specific portion of results is to be returned. Offset pagination is usually paired with sorting to make it easier for users to paginate through voluminous data sets.
	
	In this example, we're requesting a list of 10 products starting from the 21st product (since offset is 20-based). We're using the limit parameter to specify the maximum number of items we want to return, and the offset parameter to specify the starting point of the result set.

- *Cursor-based Pagination:*
	common technique used in RESTful APIs for paginating through large sets of data. In this technique, a cursor is used as a pointer to a specific location in the data set, and the API client retrieves the next page of results using the cursor
	
	**Step-1:** The API client makes an initial request to the server, specifying the number of items to be returned per page and a starting cursor value.
	`GET /users?limit=50&cursor=0`
	
	**Step-2:** The server returns the first 50 user profiles, along with a cursor value to use for the next page.
	
	**Step-3:** The API client makes a subsequent request to retrieve the next page of data, using the cursor value returned by the server.
	`GET /users?limit=50&cursor=eyJpZCI6MzQ2NTAsInNlcXVlbmNlIjozNTYyMH0=`
	
	**Step-4:** The server retrieves the next 50 user profiles from the database, starting from the position indicated by the cursor value. It then returns the next page of results, along with a new cursor value to use for the next page.
	
	**Step-5:** The process repeats until all data has been retrieved.
	Cursor-based pagination is a flexible and efficient way to paginate through large sets of data, and it can be customized to handle different sorting and filtering requirements.

- *Keyset Pagination:*
	Keyset pagination is used to retrieve the next set of results in a sorted data set. To use keyset pagination, the results must be sorted by one or more columns, and each item in the result set must have a unique identifier that can be used to determine the next set of results.

- *Seek Pagination:*
	Seek-based pagination is used to retrieve a subset of results in a sorted data set. It works by specifying a starting point and returning results that come after that starting point, up to a certain limit. Seek-based pagination is often used when dealing with large datasets and can be faster than other types of pagination.

> [!note]
API Pagination implementation - Twitter -> Cursor-based Pagination
API Pagination implementation - Spotify -> Offset Pagination

Tags: #pagination #filtering

