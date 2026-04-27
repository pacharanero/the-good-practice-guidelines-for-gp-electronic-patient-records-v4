# The Good Practice Guidelines for GP electronic patient records

This is a version-controlled, web-native version of The Good Practice Guidelines for GP electronic patient records, designed to allow the updating and development of the document over time.

## History
The Good Practice Guidelines for GP electronic patient records (The GPG) were developed to disseminate good practice in electronic health care record management in General Practice. The most recent version is the GPGv4 and this was published in 2011. A number of specialists in the field have been trying since then to create the conditions necessary for the commissioning of a revision of the GPG. This process has started but only certain sections of the GPG are expected to be revised.

The existing published GPG is at https://www.gov.uk/government/publications/the-good-practice-guidelines-for-gp-electronic-patient-records-version-4-2011

* One of the problems identified in all discussions regarding the GPG revision plans over the period it has been in discussion is that nobody can agree on how to manage the authoring. None of the organisations involved can seemingly solve this issue, despite all their resources.

* The original Word documents from which the [published PDFs](https://www.gov.uk/government/publications/the-good-practice-guidelines-for-gp-electronic-patient-records-version-4-2011) were generated appear to have been **lost** through organisational churn and general lack of organisational memory within DH (now DHSC) and NHS England (which didn't exist in 2011). In an effort to preclude future losses of the original manuscript the proposal is to use a repository under this GitHub organisation to house the originals in MarkDown format.

## Proposal for GitHub authoring and development

* This proposal is a 'guerrilla implementation' of the the GPGv5 update that uses GitHub for the content management making it very easy for people from **any** organisation to be involved in authoring the original manuscript.

* Text is 'mastered' in MarkDown, which is compiled using a very simple static site generator framework into a nice looking website that people can interact with. No PDFs. No protracted process to get the next update. GPGv6 will **not** take 10 years to organise.

* The manuscript of the GPG should be held in version control using Git and GitHub. Authors and editors have a number of options for updating the manuscript - directly editing online in GitHub, editing via a text editor such as VS Code, or using an alternative online editor such as [Prose.io](https://prose.io)

* GitHub enables each edit to be atomically tracked, attributes authorship properly, and provides tools to allow external contrinutions and updates to be 'pulled' into the new version, if the editors deem them suitable following review.

* Future releases of the GPG (version control of releases) will be managed using the GitHub 'releases' tooling.

* Issues (feedback on the GPG) will be managed through the [GitHub Issues](https://github.com/gp-good-practice-guidelines/the-good-practice-guidelines-for-gp-electronic-patient-records/issues) tab.

* Discussion about the GPG can be achieved through the [GitHub Discussions](https://github.com/gp-good-practice-guidelines/the-good-practice-guidelines-for-gp-electronic-patient-records/discussions) tab.

* The cost for this arrangement is zero. GitHub provides free code hosting for open source projects. The compilation step to create the readable web pages is achieved through a GitHub Action, and is also free. The hosting of the generated static site is free using GitHub Pages.

* The GPG will eventually be hosted at a custom URL.

## FAQs
* **Why GitHub?** GitHub is a code sharing repository which supports the ethos of openness required in medicine and medical guidelines. Microsoft own GitHub, however they exercise no control over the content of this guidance, in any form.

* **What if GitHub closes down/changes its terms/becomes no longer free?** It won't, but we could move the manuscript easily to any other Git repository provider, such as Bitbucket or GitLab.
