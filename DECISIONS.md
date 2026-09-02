# Decisions

A decision log: what you chose and why, in your own words.
P1 uses a file with this name and five questions; this one has one.
Answer it in two or three sentences after the live page is verified, then commit and push it.

## How you know it works

What check did you run on the live page, and what would have made that check fail?
A check that could not have failed is not a check.

I checked using the command curl fetch confirming an HTTP 200 and the sentence I wrote in the returned HTML. Also I looked at the live page for the dark blue background, yellow heading, and the sentence.

The curl check would fail if the page returned an HTTP status other than 200 or if the expected sentence was missing from the returned HTML. The visual check would fail if the background, heading, or sentence were missing or displayed incorrectly, indicating that the expected changes were not successfully deployed to the live page.