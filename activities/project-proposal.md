# Team Brainstorming and Preliminary Project Proposal

## Team Information

- Team name: NoMoreCtrlF  
- Working arrangement: Personal computers  
- Coordination method:In-person discussion and shared document, etc.

| Member | GitHub username | Personal CSC181 repository |
| :---- | :---- | :---- |
| Eddie F. Castre Jr. | eddie2252 | https\://github.com/eddie2252/CSC181-repository |
| Charlson Dale Fabrigar | foober123 | https\://github.com/foober123/CSC181\_Github\_Repository |
| Daverie A. Gomonit | Daverie | https\://github.com/Daverie/CSC181\_Repository |
| Ivan Jay A. Laguitao | Ivan  | https\://github.com/IvanJayLaguitao/CSC181-GitHub-repository |

## 1\. Brainstorming Record

\[Record at least two problem ideas per member. Add rows as needed. Identify whether each idea is based on experience, observation, a source, or an assumption.\]

| Member | Problem or inconvenience | Who experiences it? | Current approach | Basis of the idea |
| :---- | :---- | :---- | :---- | :---- |
| Eddie F. Castre Jr. | 1.Local members can’t tell how crowded the gym is before going; the small gym gets packed around 5pm  | Local gym members, including students  | Go and see (maybe ask others, not confirmed) | Observation: crowded around 6pm.  |
|  | Diyandi attendees who lose belongings can’t easily report or find them, and no lost-and-found table could be found  | Attendees who lose items; organizers and volunteers who would handle reports  | Posts on Facebook and social media, word of mouth  | Observation: couldn’t find a lost-and-found table. Source: reports on social media and word of mouth |
| Charlson Dale Fabrigar | When students are finding RRL for writing their theses. Searching for relevant thesis becomes cumbersome because metadata only uses names, dates, but not topics | College Students, High School Students | Remember surnames of researchers to find colleagues who have done similar research as the person who submitted the paper. Searching keywords on a research repository. And fill in the metadata for some repository’s paper searcher | Observation: Services like google scholar only take names as metadata \-imageboards use tags to sort media |
|  | When roads are congested during diyandi and some delivery workers have to deliver perishables, time spent in traffic could affect the quality of delivered products. Workers in particular are at risk because some businesses socialize losses and the worker faces salary deductions for delivery delays caused by traffic | Small business owners, delivery workers | Plan routes in advance and remember every corner in a road. In some cases, delivery workers have to park their vehicle away from the destination and deliver the product by foot | Personal Experience: In Diyandi 2025, I walked half a kilometer on foot to deliver ice. The ice was half-melted by the time it was completed |
| Ivan Jay Laguitao | 1\. Freshmen and visitors may struggle to find rooms, offices, and buildings on campus, especially during welcoming week and the first week of classes  | Freshmen, Campus Visitor, Students doing immersion | Asking guards or students, walking around until they find the place | Observation and personal experience |
|  | 2\. Students may get caught in the rain on the way to or from class because they forget to check the forecast or assume clear morning weather will last  | Students mostly with afternoon classes | Checking weather apps, guessing, watching news | Personal experience |
| Daverie A. Gomonit | Locating jeepney routes and stops can be confusing for visitors who are not familiar with Iligan City. | Visitors trying to go around Iligan via jeepney to visit different events and attractions. | Asking locals, scouring obscure blog posts | Personal Experience |
|  | Students want to measure something but can't due to the absence of a measuring tool. | Students, teachers, general workers | Estimation, using tools  | Personal Experience |

## 2\. Candidate Comparison and Selection

### Three shortlisted problems

| Candidate problem | Why it matters | Feasibility concerns | Access to potential stakeholders |
| :---- | :---- | :---- | :---- |
| When students are finding RRL for writing their theses. Searching for relevant thesis becomes cumbersome because metadata only uses names, dates, but not topics | Research and data collection take 4-8 weeks (https\://scholarlyhelp.com/blog/how-long-does-it-take-to-write-a-thesis/).  By introducing a more structured way for students to retrieve related literature, students can conserve time and allocate it to reading and conducting other parts of research. Secondary benefits of this search system is that students can pre-emptively check if their research topic is already done through checking a set of tags and identify their research can answer much sooner | The tag system has some concerns with maintenance and handling synonymous tags and implementation needs experiments to find a human friendly way to generate tags. Making a domain specific language for the system will need a compiler implementation as well | There are professors, college admin, and students who are reachable in various universities. College admin can answer concerns regarding its ethics as some research may contain sensitive data. Students are users of this search system. |
| Local gym members can’t tell how crowded the gym is before going, and the small gym gets packed around 6pm  | Members who arrive at peak hours may wait for equipment or cut workouts short. Knowing the current headcount and typical busy hours could help them pick better times. | The crowding is currently based on one member’s observation. The data depends on the owner and desk staff sharing counts, and the format of the sign-in log is unknown. Desk staff are busiest at peak hours, so live updates may be impractical. The fallback is member-submitted crowd reports, which only work if enough members report. A demo can use fictional counts, and no names or personal data are needed  | Gym members reachable through the team’s own gym-going peers. Desk staff that are present at the gym during open hours and can be approached. Owner or manager. |
| Freshmen and visitors may struggle to find rooms, offices, and buildings on campus, especially during welcoming week and the first week of classes  | Students who are new to the campus who don’t know where the buildings,rooms, and offices are located, especially those who come from outside the area, have fewer people to ask and less familiarity with the surroundings. Not knowing where to go may lead to arriving late or repeatedly asking guards and other students  | The problem peaks in welcoming week and the first week of classes, so it can’t be tested with new freshmen this semester. It needs accurate room and office data that someone has to keep updated. Campus maps exist, so the team must show what gap remains at room and office level. The idea currently rests on one member’s experience.  | This year’s freshmen are still on campus and can describe their first weeks. Guards and office staff are reachable on campus. Visitors are hard to reach on demand.  |

### Selected problem

When students are finding RRL for writing their theses. Searching for relevant thesis becomes cumbersome because metadata only uses names, dates, but not topics.

### Selection rationale

We picked the RRL search problem because every thesis or research paper needs a literature review, so any student writing one runs into it. Students are easy for us to reach, and advisers and school administrators are likely easy to reach, but we haven’t confirmed access to the research collections yet.  We did not select the gym crowding problem because it depends on an off-campus owner and desk staff sharing counts and rests on one member’s observation. We did not select campus wayfinding because its peak is the start of the year, so it can’t be tested with new freshmen this semester. 

## 3\. Preliminary Project Proposal

### Working project title

Tag-Based Search for Related Literature	\`

### Problem statement

People remember papers by concepts while computers store them as rows. This creates a conceptual gap where it becomes difficult when to read research without using a tracker like Zotero. One of the challenges of doing this kind of tracking is that if a researcher forgets critical metadata (e.g name, date) but remembers the concept. That researcher has to find other ways to retrieve it like backtracking using their browser history. A quality of life improvement for researchers is to change the searching model. Introduce an interface that lets the user perform relational algebra operations on tags related to a concept. An assumption that needs validation is that students are willing to adopt a domain specific tagging system.

### Proposed solution

Similar to searching for movies via genre, this search system lets its users retrieve related literature by a set of genres. Users can input a set of tags into the search bar and the solution will return papers that meet the tags.

## 4\. Stakeholder List

| Stakeholder role/group | Relationship to the project | Likely need or concern | Question to ask | Possible consultation method |
| :---- | :---- | :---- | :---- | :---- |
| Students writing  an RRL | Primary Users  who search for studies | Find relevant studies by topic without remembering authors or date | How do you find related studies for your RRL now, and what makes it slow and unreliable? Would combining topic tags be easier than keywords? | Short survey or informal interview with students who are currently writing thesis |
| Professors/Thesis adviser | Guide students’ literature searches | Workload of reviewing tags and tags that mislabel a study and send students to the wrong papers  | Would you be willing to review or approve tags for studies you supervised? | Short interview or form with advisers from a few departments  |
| College Admins | Manage the thesis collection and decide what can be shared or tagged  | Access permissions, sensitive data in some studies, who maintains tags over time  | How is the collection stored and searched now, who grants access to it, and are some studies restricted?  | Email through the department or library  |
| Authors of the published studies | Their work gets tagged and retrieved by topic  | Tags that misdescribe their study  | Would you be comfortable having your study tagged by topic and do the tags describe it accurately? | Through advisers or the department, or a short form to recent graduates  |

Stakeholder-count explanation, if needed: \[Explanation or Not applicable.\]

## 5\. Initial Scope

### Intended users and setting

The system will be used by college and high school students who search for specific studies or related literature while writing their thesis, caption, or research paper. Using a web app or browser, users select tags, and the system displays related research and links it to an external paper URL. The system will be demonstrated using publicly available paper records, with real thesis data to be integrated.

### In-scope capabilities

1. Users can browse and select from a list of available topic tags.  
2. Users can combine multiple tag operations to narrow or broaden results.  
3. Users can view a list of related research that matches the selected tags.  
4. Users can click a research entry to open its external research paper URL.

### Out-of-scope capabilities

1. Mobile application version.  
2. User accounts and login.  
3. Automatic tag generation using AI.

### Expected deliverables

1. A working prototype where users can select multiple tags and a resulting research catalog.  
2. A documentation of the application’s build history, its key features, how it works, and how people are supposed to use it.  
3. A comparative analysis of the prototype’s user satisfaction index against other leading research search engines (e.g. Google Scholar, RefSeek, Base etc.)  
4. A quantitative comparison of performance (i.e. time complexity, space complexity, portability, error rate).

### Constraints

| Constraint | Effect on the project | How the team will respond |
| :---- | :---- | :---- |
| It is impossible for us to host a research database on our own. | We are unable to fetch the information for the available research queries. | The team would have to use an API from an existing literary database. |
| Some research articles lack a tag for their specific study. | Therefore the system we proposed might return ineffective results. | A tag advisory system where the research title and abstract are run through an LLM/expert analysis to label it with the most appropriate tag. |

### Assumptions and dependencies

\[Identify at least two assumptions or dependencies and how to check them.\]

| Assumption or dependency | Why it matters | How to check or address it |
| :---- | :---- | :---- |
| Users will apply accurate and relevant tags to research articles.  | Incorrect or inconsistent tags can make search results unreliable and make it difficult for users to find relevant research.  | Test the tagging system with sample articles and compare user-generated tags with predefined or expert-reviewed tags. Provide standardized tag suggestions or categories.  |
| The research database remains updated.  | Outdated article information can lead to incomplete or inaccurate search results.  | Establish a regular database update schedule and monitor whether new articles and metadata are being added correctly.  |

### Success indicators

| Success indicator | Proposed evaluation method |
| :---- | :---- |
| Users can find relevant research articles more efficiently using tags.  | Conduct usability testing where users are given research topics and measure the time and number of searches needed to find relevant articles with and without the tagging feature.  |
| Users are able to apply and understand article tags correctly.  | Ask a group of users to tag a set of research articles, then evaluate the accuracy and consistency of their tags against predefined or expert-reviewed tags.  |

## 6\. Review and Next Steps

- **Before review**: A research search engine that allows users to add tags to research articles and search for articles based on those tags.  
- **After review**: A research search engine that uses a standardized tagging system to categorize research articles by topics, methods, fields, and keywords, with suggested tags to help users find relevant studies more easily.  
- **Reason**: The revised scope addresses the problem of inconsistent or subjective user-generated tags. Standardized and suggested tags make the search results more organized and reliable, while keeping the project feasible by focusing on article categorization and discovery rather than trying to replace existing research databases.

### Biggest remaining risk

The project depends on the tags quality. Even if the domain specific language has all complete features, tags that are mismatched can make the system return false positives. As for how tags are generated, it can either have a professor manually inserting them or an automated system that uses a combination of abstract keywords and word frequencies in the paper  
Three unanswered questions

1. Are the key words in an abstract good enough to use as tags in the case where a professor has not curated them?  
2. How are synonymous and related tags like Deep Learning and Neural Networks handled?  
3. Are users willing to learn and adopt a tag based way of searching

## 7\. Member Contribution Record

\[Record actual contributions, including ideas, discussion, analysis, drafting, checking feasibility, and reviewing the final document.\]

| Member | Ideas or analysis contributed | Drafting or review contribution |
| :---- | :---- | :---- |
| Eddie F. Castre Jr. | Suggested two problems ideas: H30 gym crowding at peak hours, based on my own observation, and a lost-and-found problem at Diyandi  Argued for selecting the tag-based search RRL because I think its more relatable since we also are going to take research sooner or later. Compared the candidates’ feasibility and stakeholder access.  | Split the remaining sections among the team through comments in the shared document.  Drafted the Section 4 stakeholder list Drafted the candidate 2 and 3 rows, the selection rationale and the working title. |
| Charlson Fabrigar | Suggested 2 problems: one related to Diyandi deliveries and the excess time consumed retrieving Related Literature for research The proposed solution came from seeing how imageboards make it easy to find a desired picture through tag unions | Wrote the problem statement, proposed solution, biggest remaining risk, and 3 unanswered questions |
| Daverie A. Gomonit | Suggested 2 problems: The Iligan Navigation System and Portable Measuring App. Introduced possible constraints that the application might run into. Define the assumptions and dependencies. | Drafted the success indicators and verifications method. Drafted the progression of the project thesis before and after proposal analysis. |
| [Ivan Jay Laguitao](mailto:ivanjaylaguitao@gmail.com) | Suggested 2 problems: freshmen and visitors struggling to find rooms, and buildings; students getting caught in the rain due to not checking the forecast  | Drafted the intended user and setting section Contributed to the in-scope and out-scope capabilities |

## 8\. References

\[List external sources used. Write None if no external sources were used.\]

## 9\. Team AI Use Declaration

Select one option:

- [ ] No generative AI tools were used by any member in preparing this submission.  
- [x] One or more members used generative AI tools. Details are provided below.

\[If AI was used, complete the table. If not, write Not applicable.\]

| Member who used AI | Tool | Purpose and sections assisted | How output was checked or revised |
| :---- | :---- | :---- | :---- |
| Eddie F. Castre Jr. | Claude | Used claude to help me expound or clear my fragmented thoughts, help turn into clearer wordings and to point out gaps and inconsistencies, I couldn't see myself. It assisted with Section 1, Section 2, Section 4 | Changed or removed claims I couldn’t support, and labeled assumptions as assumptions. Compared the drafts against our shared document and what I actually observed.  |
| [Ivan Jay Laguitao](mailto:ivanjaylaguitao@gmail.com) | Gemini | Used Gemini to clarify my ideas for the intended users and setting, and to refine the in-scope and out-scope capabilities of the proposed system. | Keep only what fits our scope. Removed anything that was not accurate or could not be supported. |

### Main prompts or interaction summary

Eddie : I asked Claude to help explain my idea about gym crowding, point out the weaknesses of each candidate problem, create a rough stakeholders table, and expound the fragmented ideas. List the gaps in the docs.

We acknowledge that AI-generated suggestions are not evidence of actual stakeholder interviews, feedback, or verified community needs. We remain responsible for the accuracy and explainability of this submission.

## 10\. Team Confirmation

We confirm that this document reflects our team's agreed-upon proposal. All members listed below reviewed the final version, and each member will upload the same Markdown file to their personal CSC181 repository.

| Member | Reviewed final version |
| :---- | :---- |
| Eddie F. Castre Jr. | Yes |
| Daverie A. Gomonit | Yes |
| Ivan Jay Laguitao | Yes |
| Charlson Fabrigar | Yes |

## Submission Checklist

- [x] Each member contributed at least two problem ideas.  
- [x] Three candidate problems were compared.  
- [x] The selection rationale is included.  
- [x] The problem statement contains 100–150 words.  
- [x] The proposed solution is included.  
- [x] Relevant stakeholders and consultation questions are identified.  
- [x] The scope contains 3–5 capabilities and at least three exclusions.  
- [x] Constraints, assumptions, and success indicators are included.  
- [x] A review change and three unanswered questions are documented.  
- [x] Contributions, references, and AI use are declared.  
- [x] All members reviewed the same final document.  
- [x] Each member saved the file as `activities/project-proposal.md`.  
- [x] Each member committed and pushed their copy to their personal repository.  
- [x] Each member submitted their own GitHub file link through MOLE.