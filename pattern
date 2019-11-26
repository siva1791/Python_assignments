import csv

books = dict()
path = "Books.csv"

while(True):
    print("""
    a. Enter book details
    b. View books
    c. Search book
    d. Remove book
    e. Exit
    """)

    choice = input("Enter you choice: ")

    if choice == "a":
        book_id = int(input("Enter Book Id: "))
        book_title = input("Enter book title: ")
        book_pages = int(input("Enter book pages: "))
        book_price = float(input("Enter book price: "))

        if book_id in books.keys():
            print("Already exists")
            continue
        else:
            books[book_id] = [book_title, book_pages, book_price]
            with open('Books.csv', 'a', newline='') as csv_file:
                writer = csv.writer(csv_file)
                book_details = [book_id,book_title,book_price,book_pages]
                writer.writerow(book_details)
            continue

    if choice == "b":
        with open('Books.csv', 'r') as csv_file:
            reader = csv.reader(csv_file)
            for row in reader:
                print(row)
        continue

    if choice == "c":
        id = int(input("Enter book id: "))
        if id in books.keys():
            print(books[id])
        else:
            print("Not found")
        continue

    if choice == "d":
        id = int(input("Enter book id: "))
        if id in books.keys():
            books.pop(id)
        else:
            print("Not found")

    if choice == "e":
        break
