# Blog Tags Extension
This plugin is an extension to the [RainLab.Blog](https://github.com/rainlab/blog-plugin) plugin. This extension enables tagging blog posts and displaying related articles.

### Related Posts
The `blogRelated` component can be used to display a post's related articles. This component has three properties...

- **Slug** - The target post's slug parameter.
- **Results** - The number of related posts to display.
- **Sort by** - How to sort the related articles (by relevance, title, published date, or updated date).
- **Order** - Direction to sort the results (ascending or descending).

### Tag List
The `blogTags` component is can be used to display a list of all tags. The following properties can be used customize the order and number of results to display.

- **Hide orphaned tags** - Hides tags with no associated posts.
- **Results** - The number of tags to display.
- **Sort by** - How to sort the tags (by number of posts, title, or created date).
- **Order** - Direction to sort the results (ascending or descending).

### Tag Search
The `blogTagSearch` component returns all posts with a particular tag. This component has only four properties...

- **Tag** - The URL parameter used to search for posts.
- **Paginate results** - Determines if the results are paginated or not.
- **Page** - The URL parameter defining the page number.
- **Results** - Number of posts to display per page.

This component also provides several pagination variables. They are ```totalPosts```, ```postsOnPage```, ```currentPage```, ```resultsPerPage```, ```previousPage```, ```nextPage```, and ```lastPage```. For an example of how to paginate your results, please review the pagination partial. The posts may be loaded through the ```Page``` URL parameter, or through the AJAX framework via the ```onLoadPage()``` method.
