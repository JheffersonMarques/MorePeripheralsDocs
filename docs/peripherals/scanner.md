# Scanner
---

Allows computers to read the data from written books, book and quills, printed pages and printed books

| Functions | Description |
| - | - |
| [getPage(page)](#getpagepage) | Gets the written text from the page |
| [getAuthor()](#getauthor) | Gets the author of a written book |
| [getTitle()](#gettitle) | Gets the title the scanned item |
| [getCopyStatus()](#getcopystatus) | Gets the state of a written book |

### getPage(page)
---
**Description**

Gets the written text from the page

**Parameters**

1. page: number - The page index to get

**Returns**

1. boolean - The state of the operation
2. string - The text from the book, or an error message

### getAuthor()
---
**Description**

Gets the author of the book (only supported on written books)

**Returns**

1. boolean - The state of the operation
2. string - The author of the book, or an error message

### getTitle()
---
**Description**

Gets the title of the book (supported by written books, and printed pages/books)

**Returns**

1. boolean - The state of the operation
2. string - The Title of the book, or an error message

### getCopyStatus()
---
**Description**

Gets the copy status of the book (only supported by written books)

> 💡 IMPORTANT
> 
> The values for the copy status are returned as such `"ORIGINAL", "COPY", "COPY OF COPY"`

**Returns**

1. boolean - The state of the operation
2. string - The copy state of the book, or an error message