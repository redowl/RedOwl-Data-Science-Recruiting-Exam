RedOwl Data Scientist Technical Exam, in the R language
=======================================================

To apply for a position at RedOwl Analytics, please visit
the [RedOwl Careers page](http://redowlanalytics.com/careers/)

To complete the exam, ask the Data Science team to create a private
fork of this repo for you, and then complete the following
instructions:

Composing an R script
--------------------

Fill in the R script summarize-enron.R (an empty file is provided) that
can be run from the [Unix] command line in the format:

```
> Rscript --vanilla summarize-enron.R enron-event-history-all.csv
```

The Enron event history (.csv, adapted from the widely-used publicly
available data set) is included in this repo. The columns contain:
time, messageID, sender, recipients, topic, mode where time is Unix
time (in milliseconds), the topic is usually/always empty, and the
recipients are pipe-separated. A header row is not included in the
file.

The R script should produce three outputs:

1. A .csv file with three columns---"person", "sent",
"received"---where the final two columns contain the number of emails
that person sent or received in the data set. This file should be
sorted by the number of emails sent.

2. An image file (JPEG or PNG recommended) showing a visualization of
the number of emails sent over time by some of the most prolific
senders in (1). There are no specific guidelines regarding the format
and specific content of the visualization---you can choose which and
how many senders to include, and the type of plot---but you should
strive to make it as clear and informative as possible, making sure to
represent time in some meaningful way.

3. An image file in a format similar to (2) that shows, for the same
people, the number of unique people/email addresses who contacted them
over the same time period. The raw number of unique incoming contacts
is not quite as important as the relative numbers (compared across the
individuals from (2) ) and how they change over time.


Submitting your code
--------------------

When you're done, make sure your script (but not the output) is
committed and let your contact at RedOwl know via email or "pull
request".

Code will be assessed based on completion of the tasks, efficiency,
readability, and adherence to common coding practices that best enable
sharing, re-using, and extending the code. The images need not be
sophisticated, but they should be well-organized, easily
interpretable, and of a quality typically seen in technical reports or
scientific papers.