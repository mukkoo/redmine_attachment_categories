# redmine_attachment_categories

Plugin for Redmine. Add free configurable categories to attachments. In all attachment views the category tag is shown next to the filename or the thumbnail. 

![GIF that represents a quick overview](/doc/Overview.gif)

### Use case(s)

* Mark attachments as "confidential"
* Mark attachments as invoices, which must not be forgotten
* Mark an attachment the way you want it

### Install

1. go to plugins folder

`git clone https://github.com/HugoHasenbein/redmine_attachment_categories.git`

2. go to redmine root folder

`bundle exec rake redmine:plugins:migrate RAILS_ENV=production NAME=redmine_attachment_categories`

3. restart server f.i.  `sudo /etc/init.s/apache2 restart`

### Uninstall

1. go to redmine root folder

`bundle exec rake redmine:plugins:migrate RAILS_ENV=production NAME=redmine_attachment_categories VERSION=0`

2. go to plugins folder

`rm -r redmine_attributes_quickies`

3. restart server f.i.  `sudo /etc/init.s/apache2 restart`

### Use

* Go to Administration and find a new Attachment Categories Link. Click Attachment Categories and edit existing categories or create new one by providing a name and a color. Save the new created Attachmnet Categories.

* in an issue click on the edit attachments link. Find to the right of the attachments dialog a new drop down list with your categories. As you choose the category changes to the left. Save your attachments.

In show issue see the category tag next to the attachment.

**Have fun!**

### Localisations

* English
* German

### Change-Log* 

**1.0.1** Running on Redmine 3.4.6