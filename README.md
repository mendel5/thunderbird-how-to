# thunderbird-how-to
How to configure Mozilla Thunderbird

## Config Editor

### Open the Config Editor
`Edit` --> `Preferences` --> `General` --> Scroll to bottom --> `Config Editor`

### Default sorting
Change the default sort order to "Date" with the newest e-mails on top (descending)
```
mailnews.default_news_sort_order
to 2

mailnews.default_news_sort_type
to 18

mailnews.default_news_view_flags
to 0

mailnews.default_sort_order
to 2

mailnews.default_sort_type
to 18

mailnews.default_view_flags
to 0
```

Links:
- http://kb.mozillazine.org/How_do_I_check_for_new_messages_in_other_folders

### Check all folders
Check all folders for new messages (necessary when e-mails are sorted based on the server):
```
mail.server.default.check_all_folders_for_new
to true

mail.imap.use_status_for_biff
to false
```

Links:
- https://superuser.com/questions/13518/change-the-default-sorting-order-in-thunderbird

### Encryption in transit
```
security.tls.version.min
to 4

Other options:
0 = SSL3.0
1 = TLS1.0
2 = TLS1.1
3 = TLS1.2
4 = TLS1.3
```

Links:
- https://support.mozilla.org/en-US/kb/thunderbird-78-faq
- https://www.thunderbird-mail.de/lexicon/entry/240-security-tls-version/
- https://www.privacy-handbuch.de/handbuch_31k.htm
- https://www.heise.de/news/IETF-erklaert-TLS-Urvaeter-1-0-und-1-1-als-veraltet-5997963.html
- https://datatracker.ietf.org/doc/rfc8996/
- https://datatracker.ietf.org/doc/rfc7568/

## Addons
- https://addons.thunderbird.net/en-US/thunderbird/addon/xpunge/
- https://addons.thunderbird.net/en-US/thunderbird/addon/manually-sort-folders/
- https://addons.thunderbird.net/en-US/thunderbird/addon/removedupes/


## Other
File --> Subscribe
