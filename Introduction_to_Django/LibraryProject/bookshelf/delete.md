# Delete Operation

## Command:
```python
from bookshelf.models import Book

# Retrieve the book to delete
book = Book.objects.get(title="Nineteen Eighty-Four")

# Delete the book instance
book.delete()

# Verify deletion by checking all books
Book.objects.all()
