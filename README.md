# Redgate's CORE Tech Radar

The [Tech Radar](https://radar.thoughtworks.com/?sheetId=https%3A%2F%2Fraw.githubusercontent.com%2Fred-gate%2FCORE-Tech-Radar%2Fmain%2Fradar.csv) describes Redgate's business systems landscape. We've made this repo public partly because it helps us use the technology that generates the radar, and partly because it's interesting to see the technology we use at Redgate.

If you are looking at integrating a new business tool or system, this Tech Radar gives you an idea of our current systems and how we see them within the Redgate eco-system. A separate, engineering-specific Tech Radar can be found [here](https://github.com/red-gate/Tech-Radar) - this focuses on languages, frameworks, tools and techniques for developing software at Redgate.

The [Tech Radar](https://radar.thoughtworks.com/?sheetId=https%3A%2F%2Fraw.githubusercontent.com%2Fred-gate%2FCORE-Tech-Radar%2Fmain%2Fradar.csv) describes the system landscape through a Redgate lens.  We capture systems in one of four categories:
* Infrastructure - Internal systems used by CORE to maintain and run our services.
* Third-Party - Systems that are maintained and hosted by outside vendors (e.g. Salesforce).
* Customer - Redgate systems that are customer facing.
* Internal - Redgate systems that are used by Redgaters outside CORE.

Items on the Tech Radar should only be captured if the cost of change is high or the benefits of standardizing outweigh the drawbacks. Each item on the tech radar should be there for the the good of Redgate or our customers.

Each technology choice is positioned in one of four areas.
* Explore - Investigate and understand whether it is worth persuing.
* Integrate - Should be integrated into our systems.
* Maintain - Actively used and developed.
* Deprecate - Should be eliminated, therefore only gets basic support.


We're following Thoughtworks approach. For discussion on the quadrants, please see the [Thoughtworks Radar Faq](https://www.thoughtworks.com/radar/faq)

## What isn’t on the Tech Radar?
This tech radar is not designed to cover development tools and techniques etc. Recommendations in this area are covered by our main [Tech Radar](https://github.com/red-gate/Tech-Radar). The purpose of this radar is to bring together decision-making around Redgate's business systems.

## Who builds the radar?

The radar is open for anyone within Redgate to contribute. Before contributing please read the [Contributing Guidelines](.github/CONTRIBUTING.md).

The recommended way to propose a change or spark a discussion is to open a PR. Contributions should be promptly reviewed by the CORE Lead Software Engineers or CORE Tech Leads (shout in #core-eng if this isn't the case). Comments from all other interested parties are more than welcome.

## How is the radar built?

We use [Thoughtworks Tech Radar](https://radar.thoughtworks.com/) to generate our Tech Radar. The radar is backed by a single CSV file (that should nicely [render](https://help.github.com/articles/rendering-csv-and-tsv-data/)). CSV files are parsed using `d3.js` so please see their [documentation](https://d3-wiki.readthedocs.io/zh_CN/latest/CSV) for escaping rules. All changes to the Tech Radar should be completed via a PR and merged by someone else.

You can see the latest version at [techradar.red-gate.com](http://techradar.red-gate.com).

The audience for this is anyone with an interest in Redgate's Business Systems. It's purpose is to help us to align our business software, tools and practices to build greater understanding of how Redgate works. 

## Frequently Asked Questions

### How do I contribute?
Make a PR and it'll start a conversation in #core-eng channel!

### It won't display properly. Help!

Common causes of this happening are:
* Leaving blank lines at the bottom (make sure these are removed)
* Forgetting to add a column (verify this by viewing it in GitHub's CSV display)
* Bad escaping