- Data science is not only a set of statistical and software tools and the knowledge to use them. It is also **a practice-**- a set of processes and concepts that guide the Data Scientist in making progress and decision in a data project.

-  To build a chair, you need to BOTH:

  o  Know how to use the hammers and drills and what they are.

  o  Know what to do with these tools, step by step (how and why these tools?)

- Data Science:

  o  Statistics

  o  Software

  o  Doman expertise

- Just as a good data scientist can switch domains and begin contributing relatively soon, accountants can quickly learn the financial nuances of a new industries, and a good engineer can pick up the specifics of designing various types of products.
- Domain knowledge usually takes the least time to learn well compared to statistics and software-- but I think there is a minimum threshold in which one must attain before they can formulate questions and solve them with data.
- Data centric projects-- data is the integral part of the solution for a problem. I am looking at things from the POV of the problem/goals that data can help us address.

- Issues and uncertainty in a data project that DS **must be aware of:**

  o  Data volume (too high/low)

  o  Data quality

  o  Processing speed

  o  Parameters of an algorithm (hyperparameters)

  o  Interpretability of results

- Need to notice these problems at their onset otherwise the downstream results/analysis will become invalidated, and ultimately, so will the final results/conclusions of the project.



<u>**Data project phrases:**</u>

- A data project is divided into 3 major phrases:

o  Prepare: we need more effort in gathering information at the start of the project.

o  Build: build the solution/product for the customer using statistics, ML methods, and software.

o  Finish: delivering the product, get feedback, make revision, support the product.

 

<u>**Awareness of a data project:**</u>

o  A problem is often more complex than you think. There are many considerations that must be taken into account before diving into a data project.

o  Even with nltk or spaCy, you might still face issues with the following problem.

o  To parse words from a email (ex: get all names, dates, flight number, places to infer a person's travel plans), it might involve a combination of "brute force approach", in which I match new emails to common email templates and scripts/nlp algorithm from spaCy.

- I develop some templates for the most common emails, and then compare them to a new email. I classify each new email to its closest matched template.
- Extract data from these template with spaCy.

o  The point is, even a tractable problem might contain many hidden issues that a developer will come across once he/she starts to work on it. A good DS must consider all these possibilities and try to address the ones that matters the most to a data project.

o  Awareness of problems and uncertainties in a data project and foreseeing them is one of the most valuable skills as a DS.

 

<u>**SWE vs DS:**</u>

o  SWE: If A then B

o  DS: If A then probably B (probabilistic statements about data and results)

- "I can probably use spaCy to extract travel information from a email". My solution does not work 100% of the time, so I need to define "what is good enough".
- You cannot apply a purpose-built data-centric tool to a different purpose, get bad results, and declare the tool doesn't work.

 

 <u>**Priorities**</u>

o  How I should prioritize the different concerns in a data project?

- Changing business need vs project timeline
- Data quality vs. result accuracy

 

<u>**Knowledge first, technology second, opinions third.**</u>

·  Knowledge: what you know as a fact

·  Technology: what tools you have at your disposal

·  Opinions: "almost" facts that you consider true by shouldn't quite yet.

·     Knowledge first: Know your problem, data, approach and goal before doing anything else. Keep those at the forefront of your mind.

·     Technology second: software packages are only tools that serve you, not the other way around. They shouldn't dictate your approach to the problem.

·     Opinions last: can only be use as guides (areas that I should explore).

·     **Example:** I have a method A to estimate parameters to a very high certainty, but it takes a long time to implement. I currently have method B that I can use right away, but the estimated parameters will have way more variance.

o  Solution: Use A unless A takes way too long, or too costly to implement.

o  Even if I use B, I should present results with a caveat, and pay more attention to the CI of the results to make sure it doesn't get too wide.



<u>**General Best Practices:**</u> 

·     **Don't take the goal and its attainability for granted in any data project.**

·     **In data science, a goal is much less likely to be attained in its original form.**

·     **Documentation is important!**

·     **See the whole picture first, before diving into the specifics, focus on the whole before the parts.**

 ·     **Code**

o  Comment your code

o  Even a small description of how to use the code is helpful.

o  Make sure all files have a meaningful name.

o  Use version control (git)

o  Create a new branch in Git so that your changes in the code won't break the production version.

o  Don't copy and paste code, use function or classes instead.

o  Use meaningful names for your variables.

o  Don't optimize prematurely.
 

·     **Talk to SMEs so you gain the domain knowledge that is necessary to finish a project successfully. Don't be too shy/proud.**

·     Don't use methods that are more complex than needed.

·     Make sure your "complex method" is supported/verified by simpler methods (like verify RF with logreg). Also make sure the results "make sense" intuitively.

 