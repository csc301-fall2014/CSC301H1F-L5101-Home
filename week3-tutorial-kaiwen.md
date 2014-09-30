# Case Study - Designing a Campus Book Store Application

## Initial Discussion

Design an application to facilitate buying and selling of course materials. **The application is not managed by the university.** Instead, it is a third-party application which can search for deals on new and used books from a variety of sources.

## Personas

* Average Joe
  * The average student wants to quickly find books for all his courses this semester.
* Savvy Sally
  * She wants the best bang for her bucks: she needs to easily locate the best deals for wanted books and get the best return for selling books.
* Techie Trevor
  * He wants to buy a minimum number of books: getting digital copies of course manuals to load on his reader is preferable.
  
## User stories

* Joe needs to check out a list of books for his courses (High)
* UofT needs to promote limited sales for the users of the app (Low)
* Sally wants a sales section, which can be filtered by sale percentage. The section lists books needed by Sally for her courses at the top of the page. (Medium)
* For Joe, the application needs a shopping cart which allows the user to make a single payment for all the books in the cart, regardless of the sellers. (Medium)
* For Joe, application needs to support third-party payment methods: PayPal, Bitcoins, etc. (High)
* For Sally, the application should allow used books sellers and buyers to communicate within the application without exchanging private information. (High)
* For Trevor, the eBook version should cost less than the physical version, and come with online supplementary material provided by the publisher to disincentive downloads of bootleg versions. (Low)

## Designing the MVP

The MVP should be a website which allows searches for books at various bookstores (ie. aggregator website for books). The website should be integrated with the university portal in order to retrieve the list of books the user requires for the current semester. The website should have a cart system to check out and process sales.

## First milestone release

The first milestone should be the MVP. It will first operate on an invite-only basis for friends. After feedback on the first iteration, a second round of invites will be open on the second iteration. Eventually, users of the website will be able to invite their own friends. 

## Architecture and timeline

* Web server: the web server will take a month to complete, as it is the core of the development.
* Front end: the front end can be realized in one week.
* Database: Setting up the database and initializing it should not take longer than a few days.
* Portal integration: This can be difficult to ascertain depending on the University management as we require the portal to expose an API. May take a few weeks.

## Comparison with [Kampuso](http://www.kampuso.com/)

* Kampuso is not integrated with the University portal and uses barcode scanning instead to identify required books.
* Kampuso only allows for specific books to be searched (no browsing capability). It is therefore focused on buying/selling specific books required for this semester.
* Kampuso is an iOS app only, while we were aiming for a website to reach a larger audience.
* Kampuso does not have a cart system. Instead it only provides a way for buyers and sellers to connect and complete their transaction externally. We envision an unified payment system for all the books you need. Our system will then separately distribute the payment to the various sellers.

