Are you bored of the seeing the same jobs on linkedin but don't want to block content?
Are you fed up with the twice a week reposted ones?
The ones that come again after changing to the next page?
Use the proper

## linkedin job scraper tool!
By regularly running this code([^1]), you will see only the positions, that
- match the filters([^2]) AND
- new or changed since last run.
- the positions with the same description are batched

So it can spare time and attention. The original filters e.g. check
- if the position is remote OR
- hybrid within the set countries/cities
- description has the remote keyword
you can also create your own filters easily, feel free to PR or issue ideas

## Install
1. Create a few job searches on the site, click to add alerts.
2. Install selenium in python. Any working setup from python 3.8 and above should work.
3. Set the configuration ini file to get a selenium window opened by the code.
4. First run should be `injobot.py login` that only starts selenium and opens linkedin.
5. If you login, the profile option saves the cookies and the tool can access your alerts and can search.

## Run
1. Run the tool regularly([^1]), the code scrapes even with the window not being active.
2. Check the results in the exported html output([^3])

If internet connection suxx (other error maybe?) and run gets stuck, feel free to stop it:
- the notifocation links are saved temporarily, so is the results of the processed ones
- make sure to check the results BEFORE restarting, because that will overwrite the html export with the new positions only!

Tested on linux only, feel free to PR the missing code for other platforms.

[^1]Suggested interval is one day, but should work with longer also<br>
[^2]see filters above and details in the `position.py` file<br>
[^3]it is a really simple html page, feel free to develop and PR
