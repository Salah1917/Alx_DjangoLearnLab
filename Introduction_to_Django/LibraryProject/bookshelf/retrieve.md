# Retrieve Operation

## Command:
```python
from bookshelf.models import Book

# Retrieve the book we created
book = Book.objects.get(title="1984")

# Display all attributes
book.title, book.author, book.publication_year
