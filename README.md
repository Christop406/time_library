# time_library

> This repo is forked from [matazombie/time_library](https://github.com/matazombie/time_library). Most of the below description is taken from that repository. It needs some work. Contribution instructions are at the bottom.
## Project Description
A new view of the past

I would like your help to create an app/program/webpage where a user of the app can note down and create their own library of history. 

The idea is that this can be used for any type of historical data. 
For example:
- human civilization events
- evolution of life on earth
- last two years of political events
- your personal life
- The growth of your company
- etc.

The library will be operated through a number of elements which can all interact and contain their own descriptions. Some elements will need the possibility to be nested in another.

The elements are:

**Events**

* they can be nested in one another (for example 'D-day' into 'WWII', and 'WWII' into 'post 1900', or whatever)
* any parent event can be visualized into a timeline
* they can happen:
    - over a period of time (e.g. '1810-1845'; '2/2/2011 - 2/3/2011'; '16:10 23/8/1998 - 16:15 23/8/1998')
    - at a specific moment (e.g. '316 AD'; '6/8/2001', etc.)

**Groups** (such as political parties or organisations; e.g. 'the crusaders', 'the green party' etc.)

* they can be nested in one another (e.g. 'Schutzstaffel' into 'NSDAP', or 'T-rex' into 'Dinosaurs')

**Persons**

* they can be tagged in events
* they can not be nested in one another
* they can be nested within groups (generally, or for a specified time)
* people can be related to one another (e.g. 'Otto Frank -> daughter: Anne Frank')

**Locations**

* locations can be nested in other locations (e.g. Tokio in Japan, and Japan in Asia)
* locations can change into another location over time (such as mesopotamia changed into the persian empire etc.)

**Evidence**
* these are photo's, scans or PDFs of people, objects, historical documents and studies that can be linked to any of the above mentioned elements

All elements, except pieces of evidence, can be viewed in their own timeline, in which the tagged child-events will be visualized:

**Events**
* for example, the parent event being "renaissance", the child-events being things that happened during this period

**Persons** 
* their date of birth and death can be added (both should be optional and not mandatory, in case of unknown or still alive)

**Locations** and **Groups**

Challenges:
- Timespan flexibility: events could have happened anywhere from billions of years ago until now, so to speak. In addition, early after the year 0, the yearly counting is a bit vague and sometimes whole years have been skipped. So the general timestamps and date formats may not be usefull. This issue needs to be addressed in order for the progam to be useful for any type of historical data, the most important part being able to go back in time before the year 0.
- It should be possible to view selected timelines alongside each other in order to be able to relate one element to another (e.g. what was happening in China when J.F.K. got shot)
- It should be possible for events to have vague beginnings and ends (this is especially important for events that happened a long time ago)

Other ideas:
- Along the course of history, and around different areas, different calendar types may have been or still be used, it would be nice if the user could switch to different calendar types (e.g. the islamic calendar)
- It would be nice if the user could visualize relations between people in interactive family trees

# For Developers

## Running the code
To run the code in `index.ts`, please run the command `npm start`. This will automatically run any code in the file and compile all of the typescript to the `dist/` directory.

## Contributing

To contribute to the project, please create a new branch with your proposed changes and submit a pull request explaining the changes you've made.

Note: Please merge the latest changes into your branch before submitting your pull request, or update it after the fact. Branches with merge conflicts will not be merged. 

## Contributor Code of Conduct

As contributors and maintainers of this project, and in the interest of
fostering an open and welcoming community, we pledge to respect all people who
contribute through reporting issues, posting feature requests, updating
documentation, submitting pull requests or patches, and other activities.

We are committed to making participation in this project a harassment-free
experience for everyone, regardless of level of experience, gender, gender
identity and expression, sexual orientation, disability, personal appearance,
body size, race, ethnicity, age, religion, or nationality.

Examples of unacceptable behavior by participants include:

* The use of sexualized language or imagery
* Personal attacks
* Trolling or insulting/derogatory comments
* Public or private harassment
* Publishing other's private information, such as physical or electronic
  addresses, without explicit permission
* Other unethical or unprofessional conduct

Project maintainers have the right and responsibility to remove, edit, or
reject comments, commits, code, wiki edits, issues, and other contributions
that are not aligned to this Code of Conduct, or to ban temporarily or
permanently any contributor for other behaviors that they deem inappropriate,
threatening, offensive, or harmful.

By adopting this Code of Conduct, project maintainers commit themselves to
fairly and consistently applying these principles to every aspect of managing
this project. Project maintainers who do not follow or enforce the Code of
Conduct may be permanently removed from the project team.

This Code of Conduct applies both within project spaces and in public spaces
when an individual is representing the project or its community.

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting a project maintainer. All
complaints will be reviewed and investigated and will result in a response that
is deemed necessary and appropriate to the circumstances. Maintainers are
obligated to maintain confidentiality with regard to the reporter of an
incident.


This Code of Conduct is adapted from the [Contributor Covenant][homepage],
version 1.3.0, available at https://www.contributor-covenant.org/version/1/3/0/code-of-conduct.html

[homepage]: https://www.contributor-covenant.org
