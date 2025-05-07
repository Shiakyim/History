# OOP Problem
## The system should include the following classes:

1. **Book**: This class should have the following attributes:
   - `title` (string)
   - `author` (string)
   - `ISBN` (string)
   - `isCheckedOut` (bool)

   The class should include:
   - A constructor to initialize the attributes.
   - A method `checkOut()` that sets `isCheckedOut` to true.
   - A method `returnBook()` that sets `isCheckedOut` to false.
   - A method `getDetails()` that returns a string with the book's details.

2. **Library**: This class should manage a collection of `Book` objects. It should have:
   - A private vector of `Book` objects.
   - A method `addBook(const Book& book)` to add a new book to the library.
   - A method `checkOutBook(const string& ISBN)` that checks out a book by its ISBN.
   - A method `returnBook(const string& ISBN)` that returns a book by its ISBN.
   - A method `listAvailableBooks()` that prints the details of all available books (not checked out).

3. **User **: This class should represent a user of the library. It should have:
   - `name` (string)
   - `userID` (int)
   - A method `borrowBook(Library& library, const string& ISBN)` that allows the user to borrow a book from the library.
   - A method `returnBook(Library& library, const string& ISBN)` that allows the user to return a book to the library.

**Requirements:**
- Implement the classes with appropriate access specifiers.
- Ensure proper memory management and avoid memory leaks.
- Demonstrate polymorphism by creating a derived class `Member` that inherits from `User ` and adds an attribute `membershipLevel` (string) with a method to display user details including membership level.

**Bonus Challenge:**
- Implement exception handling for cases where a user tries to check out a book that is already checked out or return a book that was not checked out.

**Submission:**
- Provide a complete C++ program that implements the above classes and demonstrates their functionality through a simple menu-driven interface.