This is for Confluence

Problems:
1. Level of specifications of the stories quite differs from story to story, from team to team. Sometimes it is too technical and too mach detailed, sometimes it's poor.
2. Feature lifecycle is not clear. Not clear who (architects, security, BA) should make his opinion on feature.
    Splitting on stories is done by PO who is not an expert in dev/QA estimations and sometimes it's need to split feature again to make it fit into iteration/release.
3. Poor bugs/improvements/stories/features structure. Hard to understand, for example, which feature improvement relates to.
4. Impossible (or very hard) to understand history of changes of the feature. For example, very hard to understand what accounting reporting should be able to do at June of the last year.

Solutions:
1. Make level of the specification more or less standard. (this document is a proposal)
2. Change feature lifecycle to make it more transparent. Identify what project roles should review feature/story on each step. Use different tools for different purposes.
Use Jira as feature/issue state tracker but not as documentation (definition, AC) holder.
3. Create a feature documentation structure. As a tree or filesystem. Each feature is a document (file) of particular version. Files can have references on each other.
 Release is a container of the features with versions.
    Gagil
        Limits 1.0
        Gold reseller 1.0
    Tomil
                Campaigns 1.0
                Gold reseller 2.0
    Rumung
            Campaigns 2.0
            Gold reseller 3.0
            Limits 2.0

4. Work with feature documentation same as with code. Work with version control to save the history and branch feature tree for the releases.

(branch diagram here)


Work with doc like with code (branch merge etc.)
Issue/progress tracking.

Main idea is that feature, epic, story are the documents (in sense of documentation) and not issues (tasks) in issue tracker.
Responsible for the complete document and its status is PO, also PO coordinates work of different roles.

1. What is the feature? What is main idea of the feature?  One - several sentences. PO
2. What feature should do? Concrete cases if possible. One - few main cases of using the feature. PO with help of BA, context DFD* if needed.
3. What subfeatures/parts this feature has? Where to place then in the system? Short description. BA with help of PO and Arch. As much independent subsystems as possible.
Then split feature into subfeatures. BA with help of PO, Arch.
For each subfeature:
3. What main processes? BA, with architects - context diagram or/and level 1 DFD if needed
4. What security risks feature has? - secutiry with help of Arch
5. What performance risks feature has? - performance team with help of Arch

*DFD - data flow diagram.

6. Use cases/stories - DEV and QA  with help of UI, usability, PO - any dev documentation if needed.
7. Test cases QA and DEV with help of PO - any QA documentation if needed.

Issues:
If use .md format - client for md markup.
