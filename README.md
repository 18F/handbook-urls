# 18F Handbook URLs

A URL shortener to use in conjunction with our [18F Handbook](https://github.com/18F/handbook/). 18F is in the process of wrapping our arms around our existing documentation &mdash; we&rsquo;ve got a lot of it &mdash; and migrating it all to GitHub. In the process, links get broken and people aren't sure where to look. A URL shortener gets around this by providing us with a single, canonical source for information that will eventually live in the handbook.

An index of the documentation pages [can be found here](https://github.com/18F/handbook#readme).  

## Installation

This is a Jekyll project, so you'll need to make sure you have [Jekyll installed](http://jekyllrb.com/docs/installation/). Then you should be able to:

1. `git clone git@github.com:18F/handbook-urls.git`
2. `cd handbook-urls`
3. `jekyll serve`

The site will then be available at [http://127.0.0.1:4000](http://127.0.0.1:4000).

## Creating a URL

Simply add a new page to the `urls` directory and follow the format of other pages. 

The current list of URLs is:

```
18f-classes
acano
accessibility
amazon-web-services
anyconnect
appearin
atom
benefits
buddy-handbook
checklist
chicago
classes
code-of-conduct
concur
consulting
core-values
dc
design
dev
distributed
docker
engineering
equipment
federal-records
general-contacts-and-listservs
getting-started
git
github-and-18f-site
github
glossary
gmail
google-calendar
google-docs
google-drive
google-hangouts
gsa-tools-equipment-and-transit
guides
hatch-act-foia-ethics-code-of-conduct
hiring
history-and-values
iaa
individual-development-plans
infrastructure
intro-to-18f-consulting
intro-to-18f-engineering
intro-to-18f-infrastructure-and-devops
intro-to-18f-infrastructure
intro-to-outreach
intro-to-product-and-open-source
intro-to-the-18f-blog
intro-to-the-diversity-working-group
intro-to-writing-lab
issues
leave-telework-and-virtual-worker
meetings-and-meeting-tools
meetings
mission
murally
networks
new-york-city
nyc
offices
omnigraffle
onboarding-buddies
onboarding-checklist
onboarding-schedule
onboarding
open-source
operations
ops
org-chart
outreach
performance-plans
policies
product-lead
product
professional-development-and-training
project-intake-101
project-selection
projects
pulls
quicktime
remote-access
remote
san-francisco
secureauth-otp
security-and-privacy
sfo
slack-and-social-media
slack
social-media
sublime
talent
teams
terminal
text-editors
tock
tools
tracking-time
training
travel-101
travel
trello
twitter
ubuntu
waffle
washington-dc
welcome-from-phaedra-and-aaron
working-groups-and-guilds-101
workshops
```

### Regenerating this list

On a UNIX or OS X system, in your local clone of this repository, run the
following command:

```shell
$ ls _urls/*.md | sed -e 's@_urls/\(.*\)\.md$@\1@' | grep -v '^$' 
```

## Public domain

This project is in the worldwide public domain. As stated in CONTRIBUTING:

This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the CC0 1.0 Universal public domain dedication.

All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
