# Crud Operations

```python
# Create Operation
from bookshelf.models import Book

book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
book


# Retrieve Operation
from bookshelf.models import Book

# Retrieve the book we created
book = Book.objects.get(title="1984")

# Display all attributes
book.title, book.author, book.publication_year



# Update Operation
from bookshelf.models import Book

# Retrieve the book to update
book = Book.objects.get(title="1984")

# Update the title
book.title = "Nineteen Eighty-Four"
book.save()

# Verify the update
book



# Delete Operation
from bookshelf.models import Book

# Retrieve the book to delete
book = Book.objects.get(title="Nineteen Eighty-Four")

# Delete the book instance
book.delete()

# Verify deletion by checking all books
Book.objects.all()
