# Library Management System Task Document

### Objective
Develop a console-based library management system in Java that enables the user to add, view, delete, and search for books.

### Features to Implement
1. **Book Addition**: Allow users to add books to the system. Each book should have the following attributes:
   - ID (unique identifier)
   - Title
   - Author
   - Year of Publication

2. **View Books**: Enable users to view a list of all books currently stored in the library.

3. **Delete Books**: Provide functionality to delete a book by its ID.

4. **Search Books**: Allow users to search for books by title or author.

### Expected Outputs
- **Book Addition**: 
  ```
  Enter book details:
  ID: 1
  Title: The Great Gatsby
  Author: F. Scott Fitzgerald
  Year: 1925
  Book added successfully!
  ```

- **View Books**:
  ```
  Library Catalog:
  ID: 1, Title: The Great Gatsby, Author: F. Scott Fitzgerald, Year: 1925
  ID: 2, Title: 1984, Author: George Orwell, Year: 1949
  ```

- **Delete Books**:
  ```
  Enter the ID of the book to delete: 1
  Book deleted successfully!
  ```

- **Search Books** (by title):
  ```
  Enter title to search: 1984
  Search Result:
  ID: 2, Title: 1984, Author: George Orwell, Year: 1949
  ```

### Implementation Hints
1. **Book Storage**: Use an `ArrayList` to store book information. Each book can be an instance of a `Book` class containing ID, title, author, and publication year as fields.

2. **Unique ID**: Ensure each book has a unique ID. You can achieve this by incrementing a static variable each time a book is added.

3. **Deleting a Book**: When deleting a book, search the `ArrayList` for a book with the matching ID. If found, remove it from the list.

4. **Searching for Books**: Implement two separate methods to search by title and author. These methods should iterate over the `ArrayList` and print details of books that match the search criteria.

5. **User Interface**: Use the `Scanner` class to read user input from the console. Implement a simple text menu that loops continuously, allowing the user to select an action (add, view, delete, search) until they choose to exit.

### Bonus Challenges
1. **Input Validation**: Add checks to ensure that the user inputs are valid. For example, the year of publication should be a four-digit number, and the ID should not be duplicated.

2. **Persistent Storage**: Extend the application to save the library catalog to a file and load it when the application starts. This involves learning about file I/O in Java.

3. **Advanced Search**: Implement more sophisticated search functionality, such as partial matches (e.g., finding a book by a substring of its title or author).

### Deliverables
- **Source Code**: Java files that include the main application and any other classes you create (e.g., `Book.java` for book objects).

- **README**: A document explaining how to compile and run your application, along with a brief description of how it works.

Remember, the goal of this task is to practice Java fundamentals such as classes, objects, collections, and basic I/O, as well as to start thinking about simple system design and user interaction through the console. Happy coding!
