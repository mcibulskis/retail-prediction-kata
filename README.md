# Retail Prediction Kata
---
## Purpose
The purpose of this kata is to begin an analysis of a provided data set, such
that you will be able to suggest a strategy for solving the business' problem
and can supply appropriate information to allow you to work with a development
team so that the solution can be implemented.

### What We Are Looking to Understand
More specifically, we are looking to get some idea of the following things in
more depth than we would be able to during a short, in-person interview:

* How do you approach problems?
* What kinds of options you consider and how you decide to pursue some and
  abandon others?
* Your consideration of the business' needs, how you might interact with the
  business, and how that plays into your thought process
* The kinds of artifacts that you typically produce as part of collaborating on
  or creating a proposed solution
* The kinds of artifacts that you typically produce to facilitate collaboration
  with a development team


---
## Format and Expectations
This exercise is presented in the format of a scenario with a mock client, the
description of which is contained later in this document.

### Time Box

* The suggested time box for working on this exercise is **7 calendar days**,
  regardless of how many total hours are spent on the exercise.

We fully expect that the exercise will not be "completed" within the
suggested time box.  Most important to us is that you provide enough to give
us insight into how you work and think through problems (see the list of
things we are looking to understand above).

If you provide artifacts that are only partially "complete" (compared to what
you would normally produce and use), please note that and describe how they are
different from what you would normally produce and use.

### Supplied Data
The mock client has supplied an initial data set for use, which you can obtain
from Kaggle with a free account.

* Data Set from Kaggle: https://www.kaggle.com/carrie1/ecommerce-data

The data set is reasonably clean and is real data from an actual ecommerce
website.

### Produced Artifacts
All produced artifacts should be submitted via a link to one of your public
[GitHub](https://www.github.com) or [BitBucket](https://www.bitbucket.org)
repositories.

*(If you do not have a GitHub or BitBucket account, you can register and have
public repositories for free.)*

* **Code:**  Any code that is produced for this exercise should be committed
  to your GitHub or BitBucket repository.
* **Written Answers/Discussion:** The suggested format for written answers or
  discussion to any of the questions (see below) is either as a plain text file,
  markdown file, [LaTeX](https://www.latex-project.org) file,
  or [Jupyter Notebook](http://jupyter.org) in your GitHub or BitBucket
  repository.
* **Other Artifacts:**  If there are other artifacts that you would like to
  show, because they are a part of your typical way of collaborating on,
  creating, or discussing a proposed solution, please also include those in
  your GitHub or BitBucket repository, along with any specific instructions for
  viewing and interacting with those artifacts.
  * *Please note that artifacts requiring the use of paid tools or
    software may be recognized as being present, but may not be examined, due to
    a lack of appropriate license for the tool/software.*
* **Other Notes:**  Any other information that you would like us to take into
  consideration, including any notes about "incomplete" artifacts
  (compared to what you would normally produce and use), with descriptions of how
  they are different from what you would normally produce and use.  Again, these
  notes should be included as either plain text files, markdown files, LaTeX
  files, or part of your Jupyter Notebook in your GitHub or BitBucket repository.

### Questions/Topics for Discussion
There are not necessarily "right" or "wrong" answers to these questions/topics.
We use your answers to assist with better understanding how you work and how
you are approaching creating and collaborating on the solutions you are
proposing.

Please answer all questions/topics for discussion in the context of the
scenario with the mock client (see below).

1. Which features are important in the data that is provided? How did you
   select them?  What justification do you have for their usefulness?

   Which features are unimportant?  Why?

1. Do you have sufficient data and information to accomplish what the mock
   client is requesting?

   If not, what other data or information would you want to ask for, and why
   would you want it? In other words, what would having that data or
   information allow you to do that you otherwise would not be able to do?

   What if you cannot get that data? (The client does not have it or is
   unwilling to supply it.)  What can you do with the data that you
   have, and what are the limitations on what you can do with it?

1. Given what you have available, what algorithms or techniques are you
   going to use?  Please demonstrate that they perform sufficiently well for
   the mock client's requests.

1. Which of your generated artifacts would you use when collaborating with
   the development team to implement your proposed solutions?  How would you
   use them, and what value do they bring in using them in those ways?

---
## Scenario
*Disclaimer: This is an imaginary scenario with a mock client.  Any perceived
similarity to actual companies or company needs, whether they are past or
future clients, is coincidental and completely unintentional.*

A new client, Interesting Goods, International, has approached us asking for
assistance, to help them better predict some of their needs.  They are based
in the UK, but sell and ship internationally to customers in multiple
different countries, most of whom are resellers or wholesalers.

They have been growing significantly over the past few years.  As a result, they
have been looking for ways to streamline their inventory management and improve
customer satisfaction.  Their goal is to reduce various costs, such as having
too much inventory on hand (increasing overhead and reducing available cash
flow) and having too little inventory on hand (incurring the cost of having
to expedite shipping from their suppliers and to their customers).

They have collected, and will be supplying to us, sales data for the past 12
months.  (Data available [here](https://www.kaggle.com/carrie1/ecommerce-data).)

The two primary problems that they would like to solve are:

1. **Streamline inventory management:**  They would like to be able to better
   predict demand for products so that they have sufficient time to re-order items
   to ensure that they are available for when customers order them.  At the same
   time, they would like to minimize the amount of inventory that they keep on-hand
   in order to maximize their available cash flow.

2. **Simplify customer re-ordering:**  A significant portion of the customer
   base are repeat customers.  While there is variation in orders, there are
   some items that are repeatedly purchased.  The client believes (but has
   not yet done any kind of statistical analysis to justify the belief) that
   adding a feature to the website to suggest that customers re-order items
   that they commonly purchase would simplify the customer's experience and
   increase their satisfaction, resulting in increased customer loyalty,
   retention, and sales.

A secondary problem that the client would like to solve is:

1. **Selection of locations for distributed warehouses:**  As the client
   continues to grow, they would like to be able to intelligently select
   locations for small "warehouses", at which they could store and ship very
   common items to nearby countries, thus reducing shipping costs for their
   customers.  This would increase customer satisfaction, resulting in increased
   customer loyalty, retention, and sales.  The client would like these
   locations to be relatively small, containing only the most common items
   ordered by companies in the nearby countries, with the main warehouse in
   the UK storing and shipping the remaining less-commonly ordered items.
   At the same time, they would like to minimize the number of these additional
   warehouses, because each warehouse comes with increased overhead costs
   in terms of facilities, personnel, shipping costs, etc.

Because new products are added over time, demand for products changes over time,
and products are seasonally removed from the product line, a one-time, static
analysis for any of the client's stated problems will not be sufficient for
their needs.  They require a system (or systems) that will continue to adapt to
changing product lines, customer demand, and continued growth of their company.
