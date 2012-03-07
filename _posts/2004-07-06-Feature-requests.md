---
layout: post
title: "Feature requests"
category:
tags: []
---
{% include JB/setup %}
I need to add the following features into news shaker to make it more usefull:

Done (has an X if finished):
  X    * Delete category and all related sites
  X    * Delete category place all remaining sites in another category
  X    * Ability to have one category be a sub category of another
        * 2 level categorization (related to the sub category idea above)
  X    * Automated "real world" testing with accuracy for all categories after a new model build. Should consist of 20 unseen and unmodeled sites that are hand categorized and then have them categorized.
  X    * A way to save the results from the real world testing in the database and display them.
        * A way to post articles that aren't links but are actually html files into the system. (This also allows visitors to view this file.)
  X    * ability for people to vote for a file that is in the wrong category to be recategorized
  X    * Increased categorization speed
        * Start a test from a new UID and then track where all the results go and view each result individually.
        *  Making sure that two of the same sites are never added to the database
        *  Checking and updating sites and getting rid of no longer existant ones.
  X    *  Ability for users to report errors and admins to view them and delete
  X    *  Ability for users to request categories and admins to view them and delete
  X    *  Ability for administrator to recategorize based on users votes to recategorize
On another note i have increased accuracy on testing to the 94% overall accuracy on known documents and i am getting and average of 25% for unknown documents, which isn't horrible but i would like to do much better. I have now began to study and look into a transductive approach that i might begin to use, depending on the results of the next bits of testing.