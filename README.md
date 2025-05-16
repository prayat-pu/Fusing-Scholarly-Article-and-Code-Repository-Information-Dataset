# Fusing-Scholarly-Article-and-Code-Repository-Information-Dataset
This repository contains a curated dataset aimed at exploring the relationships between scholarly research articles and their corresponding software code repositories (e.g., GitHub).
The complete dataset can be accessed at [https://drive.google.com/drive/folders/1Yj5melSjw8a8JI1X0Imo61pzfdSzW6cF?usp=drive_link](https://drive.google.com/drive/folders/1Yj5melSjw8a8JI1X0Imo61pzfdSzW6cF?usp=drive_link).



This file, `Dataset for Fusing Scholarly Article and Code Repository Information.csv`, contains a rich dataset designed to link scholarly publications with their corresponding code repositories. It aims to facilitate research and analysis in areas such as:

* **Reproducibility of Research:** Understanding the availability and characteristics of code associated with published papers.
* **Impact of Code on Research:** Exploring the relationship between code repository activity and the impact of scholarly work.
* **Software Engineering in Academia:** Analyzing the development practices and characteristics of research-related software.


## Column Descriptions

The dataset includes a wide range of features extracted from various sources, including Papers with Code (PWC), Semantic Scholar Academic Graph (S2AG), and GitHub (GHT). Below is a detailed description of each column:

**Papers with Code (PWC) Information:**

* `pwc_paper_url`: URL of the paper on Papers with Code.
* `pwc_paper_arxiv_id`: arXiv ID of the paper, if available.
* `pwc_paper_url_abs`: URL to the abstract of the paper.
* `pwc_paper_url_pdf`: URL to the PDF of the paper.
* `pwc_repo_url`: URL of the associated code repository on Papers with Code.
* `pwc_mentioned_in_paper`: Boolean indicating if the repository is explicitly mentioned in the paper.
* `pwc_mentioned_in_github`: Boolean indicating if the paper is mentioned in the GitHub repository.
* `pwc_abstract`: Abstract of the paper.
* `pwc_proceeding`: Publication venue or proceeding of the paper.
* `pwc_authors`: Authors of the paper.
* `pwc_tasks`: Tasks or problems addressed by the paper and code.
* `pwc_date`: Date of the paper.
* `pwc_methods`: Methods used in the paper.
* `pwc_framework`: Frameworks or libraries mentioned on the PWC page.

**Semantic Scholar Academic Graph (S2AG) Information:**

* `s2ag_id`: Semantic Scholar ID of the paper.
* `s2ag_authors`: Authors of the paper (from Semantic Scholar).
* `s2ag_inCitations`: Number of incoming citations to the paper (from Semantic Scholar).
* `s2ag_outCitations`: Number of outgoing citations from the paper (from Semantic Scholar).
* `s2ag_year`: Year of publication (from Semantic Scholar).
* `s2ag_s2Url`: Semantic Scholar URL of the paper.
* `s2ag_sources`: Sources from which Semantic Scholar obtained the paper information.
* `s2ag_pdfUrls`: List of PDF URLs for the paper (from Semantic Scholar).
* `s2ag_venue`: Publication venue (from Semantic Scholar).
* `s2ag_fieldOfStudy`: Field of study of the paper (from Semantic Scholar).
* `s2ag_magId`: Microsoft Academic Graph ID of the paper.

**GitHub (GHT) Information (based on `pwc_repo_url`):**

* `GHT_pj_id`: Project ID on GitHub.
* `GHT_url`: GitHub repository URL.
* `GHT_owner_id`: GitHub user ID of the repository owner.
* `GHT_name`: Name of the GitHub repository.
* `GH_description`: Description of the GitHub repository.
* `GHT_language`: Primary programming language of the repository.
* `GHT_created_at`: Timestamp of when the repository was created.
* `GHT_forked_from`: URL of the repository this one was forked from, if applicable.
* `GHT_delete`: Indicates if the repository was deleted (likely always False in this dataset).
* `GHT_updated_at`: Timestamp of the last update to the repository.
* `GHT_forked_commit_id`: Commit ID at which the fork occurred, if applicable.
* `GHUrl`: Duplicate of `GHT_url`.
* `GHT_total_star`: Number of stars the repository has received.
* `gh_api_forks`: Number of forks of the repository (from GitHub API).
* `gh_api_repo_language`: Primary programming language of the repository (from GitHub API).
* `gh_api_repo_created_at`: Timestamp of repository creation (from GitHub API).
* `gh_api_repo_pushed_at`: Timestamp of the last push to the repository (from GitHub API).
* `gh_api_open_issues`: Number of open issues in the repository.
* `gh_api_has_issues`: Boolean indicating if the repository has issues enabled.
* `gh_api_has_wiki`: Boolean indicating if the repository has a wiki enabled.
* `gh_api_homepage_url`: Homepage URL of the repository, if provided.
* `gh_api_subscribers`: Number of subscribers/watchers of the repository.
* `gh_api_topics`: List of topics associated with the repository.
* `gh_api_readme`: Content of the repository's README file.
* `gh_api_commit`: Number of commits in the repository.
* `gh_api_repo_age`: Age of the repository in days.
* `gh_api_repo_last_push`: Time since the last push to the repository in days.
* `gh_api_user_followers`: Number of followers of the repository owner.
* `gh_api_account_age`: Age of the repository owner's GitHub account in days.
* `gh_api_user_created_at`: Timestamp of the repository owner's account creation.
* `gh_api_repo_url`: API URL of the repository.
* `gh_api_repo_networkCount`: Number of other repositories in the same network (related to forks).
* `gh_api_repo_size`: Size of the repository in KB.
* `gh_api_repo_is_fork`: Boolean indicating if the repository is a fork.
* `gh_api_repo_mirror`: URL of the mirrored repository, if applicable.
* `gh_api_repo_contributors`: Number of contributors to the repository.
* `gh_api_repo_num_tags`: Number of tags in the repository.
* `gh_api_repo_num_release`: Number of releases in the repository.
* `gh_api_user_account_type`: Type of the GitHub account (e.g., User, Organization).
* `gh_api_user_company`: Company associated with the user, if provided.
* `gh_api_user_email`: Email address of the user, if public.
* `gh_api_user_twitter_username`: Twitter username of the user, if provided.
* `gh_api_user_public_repo`: Number of public repositories of the user.
* `gh_api_user_updated_at`: Timestamp of the last update to the user's profile.
* `gh_api_repo_lisence`: License of the repository, if available.
* `gh_api_pull_request`: Number of pull requests in the repository.
* `number_of_year_repo`: Year of the repository creation.
* `number_of_year_paper`: Year of the paper publication.
* `int_number_of_year_repo`: Integer representation of the repository creation year.
* `int_number_of_year_paper`: Integer representation of the paper publication year.
* `GHT_repo_name`: Duplicate of `GHT_name`.

**README Analysis Features:**

* `readme_tag`: Potentially extracted tags or keywords from the README.

**Code Structure Analysis Features (from README content):**

* `yuanrui_num_list`: Number of lists in the README.
* `yuanrui_num_code_blk`: Number of code blocks in the README.
* `yuanrui_num_inline_code`: Number of inline code snippets in the README.
* `yuanrui_num_img`: Number of images in the README.
* `yuanrui_num_ani_img`: Number of animated images (e.g., GIFs) in the README.
* `yuanrui_has_video`: Boolean indicating if a video is embedded in the README.
* `yuanrui_num_table`: Number of tables in the README.
* `yuanrui_num_ghlink`: Number of GitHub links in the README.
* `yuanrui_has_project_page`: Boolean indicating if a project page link is present in the README.
* `yuanrui_has_license`: Boolean indicating if a license mention is found in the README.
* `yuanrui_has_model`: Boolean indicating if a model is mentioned or linked in the README.
* `yuanrui_num_module`: Number of module mentions in the README.
* `yuanrui_num_root_file`: Number of root-level files mentioned in the README.
* `yuanrui_has_data`: Boolean indicating if data is mentioned or linked in the README.
* `yuanrui_contain_docker`: Boolean indicating if Docker is mentioned in the README.
* `yuanrui_has_shell`: Boolean indicating if shell commands are present in the README.
* `yuanrui_num_code_file`: Number of code files mentioned in the README.
* `yuanrui_num_code_line`: Number of lines of code in the README.
* `yuanrui_num_copy_paste`: Potential instances of copy-pasted code in the README.
* `repo_readme_length`: Length of the README file in characters.
* `repo_description_length`: Length of the repository description in characters.

**User/Organization Related Features (from GitHub API):**

* `user_company_bool`: Boolean indicating if the user/organization has a company listed.
* `user_email_bool`: Boolean indicating if the user/organization has a public email.

## Potential Uses

This dataset can be used for various research questions, including but not limited to:

* Identifying factors that contribute to the reproducibility of research.
* Analyzing the evolution and maintenance of research software.
* Developing metrics to assess the impact and quality of research code.
* Building recommendation systems for relevant code repositories based on scholarly articles.
* Studying the adoption of software engineering best practices in academic research.

## Data Sources

The data in this file is aggregated from:

* [Papers with Code](https://paperswithcode.com/)
* [Semantic Scholar Academic Graph](https://www.semanticscholar.org/open-data)
* [GitHub API](https://docs.github.com/en/rest)


## Contact
Mr. Prahyat Puangjaktha - Prahyat.Puangjaktha@gmail.com
