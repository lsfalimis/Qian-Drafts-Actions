#Drafts Actions

##Tab 1

Name | My favour | URL | Note
-- | -- | -- | --
List in OmniFocus | + | drafts://x-callback-url/create?text={{!Reminders}}%0A[[draft]]&action={{List in Reminders}}&afterSuccess=Delete&x-success={{omnifocus://}} | Make sure: a list called 'Reminders' in Reminders.app; In OmniFocus 2.app, Settings - Reminders - On

##Tab 2

Name | My favour | URL | Note
-- | -- | -- | --
Log in Dropbox, search in Chrome and can return | #q | drafts://x-callback-url/create?text=[[selection]]&action={{log-search}}&afterSuccess=Delete&x-success={{googlechrome-x-callback://x-callback-url/open/?url=http%3a%2f%2fwww.google.com%2f%23q%3d[[draft]]&x-source=Drafts&x-success=drafts%3a%2f%2f&create-new-tab}} | Make sure: Set up 'log-search' action
Log in Dropbox, feel lucky in Chrome and can return | #q&btnI | drafts://x-callback-url/create?text=[[selection]]&action={{log-lucky}}&afterSuccess=Delete&x-success={{googlechrome-x-callback://x-callback-url/open/?url=http%3a%2f%2fwww.google.com%2f%23q%3d[[selection]]%26btnI&x-source=Drafts&x-success=drafts%3a%2f%2f&create-new-tab}} | Make sure: Set up 'log-lucky' action
Find in 1Password | 1p | onepassword://search/[[selection]] |
Log in Dropbox and open in App Store | app store | drafts://x-callback-url/create?text=[[selection]]&action={{log-appstore}}&afterSuccess=Delete&x-success={{googlechrome-x-callback://x-callback-url/open/?url=https%3A%2F%2Fwww.google.co.uk%2F%23q%3Don%2Bthe%2BApp%2BStore%2Bon%2BiTunes%2B[[selection]]%26btnI}} | Make sure: Set up 'log-appstore' action
Log in Dropbox and search in App Store | app store_s | drafts://x-callback-url/create?text=[[selection]]&action={{log-appstore}}&afterSuccess=Delete&x-success={{http://search.itunes.apple.com/WebObjects/MZSearch.woa/wa/search?media=software&term=[[selection]]}} | Make sure: Set up 'log-appstore' action

##Tab 3

Name | My favour | URL | Note
-- | -- | -- | --
Decode in TextTool, set to clipboard and return | texttool://x-callback-url/transform?text=[[selection]]&method=decode&x-success={{drafts://}} | 
Encode in TextTool, set to clipboard and return | texttool://x-callback-url/transform?text=[[selection]]&method=encode&x-success={{drafts://}} | 
Send to Command-C's 1st device | ⌘c | command-c://x-callback-url/copyText?text=[[selection]]&deviceIndex=0&x-success={{drafts://}} | Note: set up Command-C *properly*

##Tab 4

Name | My favour | URL | Note
-- | -- | -- | --
Lookup in Eudic and can return | d | eudic://dict/[[selection]]?jumpback=drafts: | 

##Hidden

Name | My favour | Import URL | Note
-- | -- | -- | --
Append to DROPBOX/Log/log-search.txt | log-search | drafts://x-callback-url/import_action?type=dropbox&name=log-search&path=%2FLog%2F&filenametype=2&filename=log-search&ext=txt&writetype=2&template=%5B%5Btime%5D%5D%20%5B%5Bdraft%5D%5D | Make sure: link Drafts.app to Dropbox
Append to DROPBOX/Log/log-lucky.txt | log-lucky | drafts://x-callback-url/import_action?type=dropbox&name=log-lucky&path=%2FLog%2F&filenametype=2&filename=log-lucky&ext=txt&writetype=2&template=%5B%5Btime%5D%5D%20%5B%5Bdraft%5D%5D | 
Append to DROPBOX/Log/log-appstore.txt | log-appstore | drafts://x-callback-url/import_action?type=dropbox&name=log-appstore&path=%2FLog%2F&filenametype=2&filename=log-appstore&ext=txt&writetype=2&template=%5B%5Btime%5D%5D%20%5B%5Bdraft%5D%5D | 