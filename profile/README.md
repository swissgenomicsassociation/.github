# Swiss Genomics Association

<https://www.swissgenomicsassociation.ch>

**Shared standards for collective health.**

Experts from across Switzerland working together to define open, evidence-based guidelines for genomics in health, research, and national practice.

* Deutsch: Schweizerische Genomik-Vereinigung
* Français: Association Suisse de Génomique
* Italiano: Associazione Svizzera di Genomica
* English: Swiss Genomics Association

## About

The **Swiss Genomics Association** is a national collaboration of volunteer experts from academia, hospitals, government, and industry.
Our goal is to define **open, evidence-based standards** for the responsible use of genomics in human health, precision medicine, and research.

We meet to identify and prioritise key topics of national importance. Each topic is developed through expert discussion, literature review, and coordination with international partners who use or contribute to the resulting standards.

Our outputs include **white papers, guidelines, and reference materials** that support consistent and credible genomic practice across Switzerland.

---

## Contribute and collaborate

Calls for members to collaborate are announced via email and posted on our release page.  
Working documents and release candidates are listed on the release page:  
<https://www.swissgenomicsassociation.ch/releases/>

We email guideline articles to our members in two stages: first to invite contributions, and later once the articles are completed.

You may contribute using **any one** of the following options:

1. Send your input by email to **admin (at) swissgenomicsassociation (dot) ch**.
2. Download the current PDF and add comments and send by email.
3. Join the next meeting call to discuss the content live.
4. Request an Overleaf link by email to comment or edit the LaTeX source.
5. Submit a pull request on the GitHub source repository.

Contributing members are named as authors. A joint acknowledgement is included for the whole Association without naming members. 

In some cases, core contributors may be added directly to the GitHub organisation.

---

### Repository structure

All work is organised across two types of repositories:

* The **main website repository** (`swissgenomicsassociation.github.io`) publishes the official releases from these projects for open access.
* **Project repositories** (e.g. `mendelian_disease_interpretation`) contain the source code, analyses, and LaTeX used to produce manuscripts or datasets.

During the website build, release files (for example, PDFs or datasets) are synchronised automatically to
`assets/release/<project_name>/latest/`, making them directly available on the public site.

Example:
[View latest release](https://swissgenomicsassociation.github.io/assets/release/mendelian_disease_interpretation/latest/mendelian_disease_interpretation_v1.pdf)

---

## Writing and syncing releases

All Swiss Genomics Association projects are developed in separate repositories under the organisation domain (<https://github.com/swissgenomicsassociation>), each producing versioned outputs such as manuscripts, datasets, or configuration files. The main website (`swissgenomicsassociation.github.io`) hosts the latest public releases from these projects and gets directed to <https://www.swissgenomicsassociation.ch>. During the site build, the `sync_releases.sh` script automatically copies current release files from their respective repositories into the website `assets/release/` directory, making them directly accessible for viewing or download, for example:
`https://swissgenomicsassociation.github.io/assets/release/mendelian_disease_interpretation/latest/mendelian_disease_interpretation_v1.pdf`.

Thus to write new release content, the main article will be developed in the organisation repo - not in the actual website repo, release page, or assets directory. For instance see <https://github.com/swissgenomicsassociation/sga_qem> which is then synced to the release page via latest assets. Only pages with supporting "about" information and website content are developed directly in the website repository by the web admin.

---

## Technical info for git users
### Join our GitHub organisation

Members who require access to github directly can request it by emailing  
**admin (at) swissgenomicsassociation (dot) ch**  
including their GitHub username or account email.

**Process**

1. Email your details to **admin (at) swissgenomicsassociation (dot) ch**
2. You will receive an invitation via GitHub under Organisation → People → Invite member
3. Accept the invitation in your email or GitHub notifications  

Invitations expire after 7 days and can be reissued.

---

### Working on content

* Contributions are usually made through branches or forks
* Changes are submitted as pull requests
* Review is required before merging into main
* Direct pushes to protected branches are limited to maintainers

Some projects also support collaboration on Overleaf or through shared editing, meetings and email where this is suitable.

---

This readme is found at `.github/profile/README.md`.
