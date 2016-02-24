# Sandra.Snow.NotesTheme
**Notes** is a theme for the static website generator [Sandra.Snow](https://github.com/FBoucher/Sandra.Snow).

Base on the default theme, **Notes** is a minimalist theme ready to use.

## How to use it

To use Sandra.Snow.NotesTheme copy the folder 'notes' in the themes folder


    root
    |-- _pages
    |-- _posts
    |-- themes
    |   |-- default
    |   |-- **notes**
    |
    |-- snow.config  
    

### Configuration

#### Set the theme

In the file 'snow.config' by sure to change the value of theme for notes

    "theme": "notes"

#### Adjust processFiles

Sandra.Snow.NotesTheme doesn't have an about page. You need to remove that section in  processFiles of snow.config file.

##### Before

    


	"processFiles": [{
	        "file": "index.cshtml",
	        "loop": "Posts"
	    },{
	        "file": "category.cshtml",
	        "loop": "Categories"
	    },{
	        "file": "categories.cshtml => category"
	    },{
	        "file": "archive.cshtml"
	    },{
	    	"file": "about.cshtml"
	    },{
	        "file": "drafts.cshtml",
	        "loop": "Drafts"
	    },{
	        "file": "feed.xml",
	        "loop": "atom"
	    }]
    
##### After

	"processFiles": [{
	        "file": "index.cshtml",
	        "loop": "Posts"
	    },{
	        "file": "category.cshtml",
	        "loop": "Categories"
	    },{
	        "file": "categories.cshtml => category"
	    },{
	        "file": "archive.cshtml"
	    },{
	        "file": "drafts.cshtml",
	        "loop": "Drafts"
	    },{
	        "file": "feed.xml",
	        "loop": "atom"
	    }]

