# elibrary
SQL database

<h2>About the E-Library</h2>
E-Library is a database of IT related e-books. Table 'ebooks' contains information about the title, authors, publisher, subject, format, number of pages, size[MB], published year and source. The current size is 126 books on 271 rows, due to the different formats. The information was collected and put into database manually, via MariaDB Server, in 14 hours. 

<h3>The 'topic' / subject column</h3>
The initial thought was to sort the books by topics or subjects. Several issues appeared. Sorting by subjects does not work because books focused on general-purpose languages can fall into multiple categories. Sorting by languages does not work either, for opposite reasons. The 'Others' category was forbidden at first. Later, it started existing for rare cases. During the final clean up, there were 27 categories, which shrank into 8 with 'Others' containing one third of the 'ebook' table. The final state is far from ideal but acceptable.

<h3>Format and pages columns</h3>
Many e-books come in multiple formats (by frequency .pdf, .epub, .mobi and .prc), each with different number of pages. Recordings were made for getting more precise data about the e-library. Three different tools were needed to open the different formats in Ubuntu. This part was the most time consuming.
