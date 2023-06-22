# Teaching Assistant Duties

Here's an attempt at summarizing the TA duties for the class when it was held this time around
(Julian Michael TAing for Yulia Tsvetkov's Ethics in NLP class at UW in Winter quarter 2022), course
website [here](https://courses.cs.washington.edu/courses/cse599d1/22wi/).
This tries to discuss everything I did (except the preparation of the Philosophical Foundations
lecture). You might not need to do all of it, and I probably missed some stuff.
Update this document accordingly if you fork the repo.

## Class Setup

Stuff you have to do once at the beginning of the quarter.

### Google Drive

Create a Google Drive folder for all of the class assignments and turnin.
* Give **edit** access to other instructors and **view** access to all students.
* Create at least a reading list (doc) and subfolder for lecture slides.
* Create a subfolder for students called, e.g., "Student Information", and give **edit** access to students. This will be used for confidential information about students and assignment turnin.

### Mattermost

Create a new "Team" within the UW CSE Mattermost instance and name it for your class (e.g., ethnlp-wi22).

### Discussion Prep

* Randomize the list of students and split them into discussion groups (we had 4 groups for a class of ~30), and provide this information in a Sheet in the Google Drive under "Student Information". These groups will last for the quarter.
* Create a Mattermost discussion channel for each group (#paper-discussion-1, #paper-discussion-2, etc.).
* Create a "Discussion Slides" subfolder under "Student Information". This will hold the slides that students will use to present summaries of their discussions.

### Website

* Set up a GitHub repository for the class website. Example repo [here](https://github.com/julianmichael/ethnlp-wi22/).
* Set up the repository to automatically deploy on push, using GitHub Actions. The workflow is in the repo [here](https://github.com/julianmichael/ethnlp-wi22/blob/main/.github/workflows/build_and_deploy.yml). 
    * Besides including the workflow file, you'll need to add two secrets to the repository:
        * `KNOWN_HOSTS` containing the courses webserver's public info. The output of `ssh-keyscan -H courses.cs.washington.edu` (running from your local machine is fine).
        * `WEBSERVER_SSH_PRIVATE_KEY` containing a private key paired to a public key in your user's `authorized_keys` on the CSE servers. It's probably prudent to generate a new key pair for this purpose.
    * You'll also need to change the last line of the workflow to use your username and class directory in the `scp` command.
* Add or update the website content:
  * Staff information in [_staffers/](_staffers/): the body can include details on office hours.
  * Class schedule in [calendar.yml](_data/calendar.yml).
  * Syllabus in [index.md](index.md).
  * Any updates to the discussion or assignment instructions in [_assignments/](__assignments/).
* Add/update links to the website for the Mattermost, Google Drive, and reading list (e.g., in the sidebar, under `quick_links` in [_config.yml](_config.yml)).

### Zoom

If using Zoom, set up a recurring Zoom meeting for the class.

### Communication with Students

Send out an introductory email to all students with at least the following information:
* Link to the course website
* Link to the Google Drive and request that people make sure they have access / ask you if they can't get in
* Invite link for the Mattermost instance
* Link to the discussion group assignments and instructions for people to join their respective Mattermost discussion channels
* Zoom link

## Regular Duties

### Site updates / announcements

Immediately before or after each lecture:
* Place the lecture slides in the appropriate folder in the Google Drive.
* Add a bookmark to the reading list doc for the next lecture/discussion's readings.
* Update the calendar with links to the new slides and readings (edit [calendar.yml](_data/calendar.yml_).)

Prior to a paper discussion section, as soon as the reading list is settled (preferably immediately after the preceding lecture):
* Create a Google Slides deck in the "Student Information" > "Discussion Slides" folder for the next discussion. All students should automatically have edit permissions.
  * Create a title slide for each paper to be discussed. Students will add slides to each section and use this deck as a visual aid for their discussion summaries.
  * Link the slides in the calendar on the course website and in the Mattermost Town Square channel.
* Set the header of each Mattermost paper discussion channel (e.g., #paper-discussion-1) to include links to that group's readings.
  * This is as a convenience to the students. If you choose to do this, then make sure to reliably do it immediately once the readings are settled, or the students will start relying on it and then miss when the readings come out (I got lazy shortly into the quarter and this happened...).

### Zoom / in-class logistics

If doing paper discussions over Zoom:
* At the discussion start, create _n_ breakout rooms, one for each group, marking the option that lets people assign themselves to their own breakout room.
* Take attendance in the first 5 or 10 minutes by looking at the Zoom participants. Keep track in a spreadsheet so you can identify if anyone hasn't been participating regularly.
* Have instructors rotate between breakout rooms (starting in different ones) spending _M/n_ minutes in each (where _M_ is the number of minutes devoted to class discussion**.
* Close breakout rooms a minute before discussions should end.
* Prompt each group's lead to share their screen and summarize their discussion.
  * Enforce time constraints as best you can, because people will naturally go over. We didn't do this well.

## Assignments

### Ethics Review

**Beginning of quarter:**
* Either do the "before assigning" work below or put `nav_exclude: true` in the front matter of the [assignment page](_assignments/ethics_review.md) until you have the details figured out.
* Decide on assignment/due dates and put them in the course [calendar](_data/calendar.yml).

**Before assigning:**
* Find papers to assign for ethics review. You can use the papers we did (in our Google Drive), or you can find new ones. The easiest way to do this is to Google search `site:openreview.net "Ethics Review of" "Ethical Issues: Yes" NeurIPS` to find NeurIPS papers, or modify to fit your conference of choice.
* Download PDFs of these papers and create copies where you redact all discussion of ethical concerns and anything that would deanonymize the paper (author names, conference information, links, page numbers). I used a free trial of PDFExpert on desktop to do this.
* Upload the redacted PDFs into a folder on the Google Drive.
* Create a subfolder in the Google Drive under "Student Information" for turnin.
* Modify the [assignment page](_assignments/ethics_review.md) as desired, including a link to the directory of redacted PDFs and a link to the turnin directory.
* Remove `nav_exclude: true` from the assignment page front matter, if applicable.
* Notify students of the assignment.

**After due date:** Create a summary slide deck to give the students feedback on their reviews and describe the actual ethics reviews of the papers.
* Place it in the Drive (e.g., under "Lectures" if you plan to deliver it as a lecture).
* Include links to the openreview forums for each paper so people can see the actual ethics reviews and original papers.
* Include a brief summary of good things the students did and things that people could have improved on. Explicitly compare & contrast them with real ethics reviewers (or encourage them to take a look). Chances are they were much better than the real ones.
* For each paper, consolidate the ethics reviews of all of the students summarize the points they raised. Then discuss how these differed from the points raised by ethics reviewers and in the final un-redacted paper.
* Deliver the feedback during class, time permitting.

### Project Proposals

* Write up specific requirements in an assignment page, e.g., [here](_assignments/project_proposal.md). I did not bother with this; we just verbally described the assignment in class. But in retrospect it would have been better to have it clearly described on the website.
* Create a subfolder under "Student Information" for pre-proposal turnin.
* Create a subfolder under "Student Information" for final proposal turnin.

**First couple weeks of the quarter:**
* Describe the assignment to students and ask them to send in pre-proposals with their groups and topic.

**After pre-proposal turnin:**
* Assign each proposal group to an instructor (e.g., in a private spreadsheet). Each instructor can provide feedback on their groups' pre-proposals via email.

**Within 1 or 2 weeks of proposal presentation dates:**
* Randomize proposal groups into a presentation schedule.
* Put it in a sheet in "Student Information".
* Instruct students to swap among themselves if they need to change times.

## Grading

* Either as the quarter progresses, or all at the end, count up the number of substantive questions/replies made by students in their Mattermost channels. This will help you identify if students haven't been participating regularly in the Mattermost.
* Combine Mattermost participation with discussion attendance to get participation grades.
* Grade ethics reviews as you see fit.
* Grade proposals and presentations as you see fit.

