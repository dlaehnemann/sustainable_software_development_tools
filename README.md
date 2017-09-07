# Tools, practices and recommendations for sustainable software development

This is an open collection of tools, methods and recommendations for sustainable software development, so please feel free to [contribute](https://github.com/dlaehnemann/sustainable_software_development_tools/blob/master/CONTRIBUTE.md). This comes from a background of open software development in science (with some inherent biases towards bioinformatics and Open Source), but is meant to contain generally applicable recommendations and tools. Wherever possible, we try to link to maintained lists and recommendations in other places.

The following structure is merely a suggestion and should change whenever thought necesseary:

# General Recommendations

## Reading and learning

* Wilson G, Aruliah DA, Brown CT, Hong NPC, Davis M, Guy RT, et al. Best Practices for Scientific Computing. PLOS Biol. 2014;12: e1001745. doi:10.1371/journal.pbio.1001745
* Wilson G, Bryan J, Cranston K, Kitzes J, Nederbragt L, Teal TK. Good enough practices in scientific computing. PLOS Computational Biology. 2017;13: e1005510. doi:10.1371/journal.pcbi.1005510
* Silva LB, Jimenez RC, Blomberg N, Luis Oliveira J. General guidelines for biomedical software development. F1000Research. 2017;6: 273. doi:10.12688/f1000research.10750.1
* the planned Open Science MOOC is meant to also cover research software / Open Source: <http://fossilsandshit.com/badassery/open-science-mooc/>

# Version control / collaborative development

`git` has become the de-facto standard for version control

## Reading and learning

* extensive `git` online documentaiton: <https://git-scm.com/>
* open Software Carpentry course material for a `git` introduction: <https://swcarpentry.github.io/git-novice/>
* Perez-Riverol Y, Gatto L, Wang R, Sachsenberg T, Uszkoreit J, Leprevost F da V, et al. Ten Simple Rules for Taking Advantage of Git and GitHub. PLOS Computational Biology. 2016;12: e1004947. doi:10.1371/journal.pcbi.1004947
* Blischak JD, Davenport ER, Wilson G. A Quick Introduction to Version Control with Git and GitHub. PLOS Computational Biology. 2016;12: e1004668. doi:10.1371/journal.pcbi.1004668

## Tools

commercial platforms:
* GitHub: https://github.com/
* BitBucket: https://bitbucket.org/
* GitLab (hosting and service cost): https://about.gitlab.com/products/

self-hosting alternatives:
* GitLab (OpenSource): https://about.gitlab.com/products/

# Code documentation

this spans a wide range, from small in-line comments explaining bits of code to documentation semantics that can be used to auto-generate documentation for developers, e.g. API-documentation

## Tools

* Doxygen (C, C++, Python, Java, ...): https://github.com/doxygen/doxygen
* Sphinx (Python): http://www.sphinx-doc.org/en/stable/
* Javadoc (Java): http://www.oracle.com/technetwork/java/javase/documentation/javadoc-137458.html
* documentation as a language feature:
  * Rust: https://doc.rust-lang.org/book/first-edition/documentation.html

# Code review

## Reading

* https://mozillascience.github.io/codeReview/intro.html
* Petre M, Wilson G. Code Review For and By Scientists. arXiv:14075648 [cs]. 2014; Available: http://arxiv.org/abs/1407.5648
1.
* MacLeod L, Greiler M, Storey M-A, Bird C, Czerwonka J. Code Reviewing in the Trenches: Understanding Challenges and Best Practices. IEEE Software. 2017; Available: http://ieeexplore.ieee.org/abstract/document/7950877/

## Tools

Code review as a practice is possible in any setting, but is usually supported by collaboration platforms (e.g. GitHub, BitBucket, GitLab).

# Testing / Continuous Integration:

very diverse range of testing (unit tests, regression tests, continuous integration, ...)

## Reading

* a general testing guide with useful Wikipedia links: <https://www.software.ac.uk/resources/guides/testing-your-software>
* unit tests with language specific frameworks: <https://en.wikipedia.org/wiki/List_of_unit_testing_frameworks>
* continuous integration of full projects: <https://en.wikipedia.org/wiki/Continuous_integration>

## Tools

* continuous integration:
  * software available: <https://en.wikipedia.org/wiki/Comparison_of_continuous_integration_software>
  * hosted solutions online: <https://www.software.ac.uk/resources/guides/hosted-continuous-integration>
  * examples:
    * TravisCI, free for Open Source projects: https://travis-ci.org/
    * Jenkins, self-hosted: https://jenkins.io/

# Build and installation automation

an automatic build and deploy mechanism, including central repositories, can greatly facilitate distribution and installation processes

## Reading

* Build automation tools: <https://en.wikipedia.org/wiki/List_of_build_automation_software>

## Tools

language-specific tools:

* pip (Python): <https://pip.pypa.io/en/stable/>
* Maven (Java): <https://maven.apache.org/what-is-maven.html>

language-specific repositories for libraries or packages:

* cran (R): <https://cran.r-project.org/>
* PyPi (Python): <https://pypi.python.org/pypi>
* docs.rs (Rust): <https://docs.rs/>
* bioconductor (R, specific repo for bioinformatics): <https://www.bioconductor.org/>

language-independent repositories for software and libraries:

* conda: <https://conda.io/docs/index.html>
  * with channels like conda-forge (general purpose open contribution channel: <>) or bioconda (bio-specific open contribution channel: <https://bioconda.github.io/>)

# Issue tracking

## Reading

* overview of issue tracking systems: <https://en.wikipedia.org/wiki/Comparison_of_issue-tracking_systems>

## Tools

* oftentimes integrated into platforms for project management (e.g. Trac, Redmine) or collaborative development (e.g. GitHub, Bitbucket)
* project management software: <https://en.wikipedia.org/wiki/Comparison_of_project_management_software>
  * OpenProject: <https://www.openproject.org/>
  * Trac: <https://trac.edgewall.org/>

# User documentation

distinct from developer/API documentation, this requires basic usability insights, and can range from useful command line help and error messages to extensive online help and tutorials, and should be versioned alongside software versions

## Tools

* Read the docs, free online documentation hosting platform: <https://readthedocs.org/>
* GitHub functionality: README.md in repositories main folder or GitHub Pages (<https://help.github.com/articles/what-is-github-pages/>)
* language-specific frameworks 

# Software licensing

## Reading

* list of Open Source licenses: <https://opensource.org/licenses>
* Morin A, Urban J, Sliz P. A Quick Guide to Software Licensing for the Scientist-Programmer. PLOS Computational Biology. 2012;8: e1002598. doi:10.1371/journal.pcbi.1002598

## Tools

* website to guide you through software license choice: <http://choosealicense.com/>
* browser-based tool to guide you through software and data license choice: <https://ufal.github.io/public-license-selector/>

# Journals for publishing software descriptions

For proper credit of the value of software development in science, it is still necessary to turn software into citable publication. This list is meant to provide developers with possible outlets:

* Journal of Open Research Software: <https://openresearchsoftware.metajnl.com/>
* Journal of Open Source Software: <http://joss.theoj.org/>
