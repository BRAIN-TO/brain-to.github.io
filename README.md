
  ![on-push](../../actions/workflows/on-push.yaml/badge.svg)
  ![on-pull-request](../../actions/workflows/on-pull-request.yaml/badge.svg)
  ![on-schedule](../../actions/workflows/on-schedule.yaml/badge.svg)

  # BRAIN-TO's Website

  Visit **[brain-to.github.io](https://brain-to.github.io)** 🚀

  _Built with [Lab Website Template](https://greene-lab.gitbook.io/lab-website-template-docs)_

  ## How it Works
  [Lab Website Template](https://greene-lab.gitbook.io/lab-website-template-docs) is built using [Jekyll](https://jekyllrb.com/) and deployed via. [GitHub Pages](https://pages.github.com/). The website is automatically deployed when changes are pushed to the `main` branch of this repository. GitHub actions are used to build and deploy the website by running a Docker container that generates the static site files through Jekyll from the markdown content pushed to the `gh-pages` branch. By design, GitHub workflow is also set to run on a schedule to auto-update the website on a weekly schedule so that Manubot may run. If a commit doesn't resolve fully, GitHub actions will fail and not update the website, this is to ensure that the live website always remains in its last working state.

  In order to gain edit permissions to this repository, please reach out to a Team Owner to be added as a member with your GitHub username or email address. This repository is set to public so that gh-pages can be generated, however only members with write access can push changes to the `main` branch.
  
  ## Intructions for new member pages
  To add your own member page to the website, please follow these steps in either of the two methods below. The first method is recommended for quick edits, while the second method is more suitable for extensive changes and local testing.
  
  ### Method 1
  Create and edit the markdown files directly on GitHub by navigating to the desired file and clicking the pencil icon to make changes. This method is recommended for small edits such as adding a new member page but lacks the ability to preview changes locally before pushing them live.
  
  1. Upload an image of yourself by uploading them to the `images` folder ideally as your `your_first_name.jpg`. For the best effect, upload a square image, or crop your image to be a square image. If you don't have one, it will default to the fallback image of a faded beaker. Take note of what you upload it so that you can reference it in your member page. Please be careful to not upload images with the same name as existing images to avoid overwriting them.
  2. Add a new member page by creating a new markdown file in the `members` folder as `members/first_name-last_name.md`, following the existing file structure and front matter format. A template can be found in `members/template-name.md` for you to duplicate and edit.
  3. More detailed instructions can be found in the [Team members | Lab Website Template Documentation](https://greene-lab.gitbook.io/lab-website-template-docs/basics/team-members).
  
  ### Method 2
  Alternatively, you can clone the repository to your local machine, make changes using a text editor or IDE (e.g, VS Code), and push your changes back to GitHub. This method allows you to preview the website locally before pushing changes live.
  
  1. Clone the repository to your local machine using git:
        ```
        git clone https://github.com/BRAIN-TO/brain-to.github.io.git
        ```
  2. Navigate to the cloned repository directory:
        ```
        cd brain-to.github.io
        ```
  3. To setup a local preview of the website, ensure you have [Docker](https://www.docker.com/) installed and running. Then, run the following command in the terminal from the root directory of the repository:
        ```
        .docker/run.sh
        ```
  4. Once the docker container is first built and running, the terminal will show you that the preview is running and the website is accessible locally by opening a web browser and navigating to:
        ```
        http://localhost:4000
        ```
  5. Make the necessary edits to the markdown files or other content using your preferred text editor or IDE using the intructions from Method 1. As you save different files, the local preview should automatically reload to reflect your changes. Sometimes the Docker container may need to be restarted to reflect certain changes.
  6. Once you are satisfied with the changes, ensure that your files are saved locally before staging and committing your changes using git. 
  7. Once committed, GitHub actions will trigger to regenerate the HTML files so that the live website will be updated.

## Editing other content
In addition to adding member pages, you can also edit other content on the website such as the homepage, projects, publications, resources, and more. Most of this should be already setup so it shouldn't require major edits but the content is organized in markdown and YAML files located in various folders within the repository. You can follow similar steps as outlined in Method 1 or Method 2 to make changes to these files. A general description of the page content and layout can be found in the [Edit pages | Lab Website Template Documentation](https://greene-lab.gitbook.io/lab-website-template-docs/basics/edit-pages).

- Homepage: `index.md`
- Research: `research/index.md` and add new project descriptions in `_data/projects.yaml`. I suggest not making this too long as it will clutter the page.
- Publications: `_data/orcid.yaml` for entering additional ORCID scrapers (most accurate) and `_data/sources.yaml` for manually adding/fixing/missing publications. More information can be found at [Citations | Lab Website Template Documentation](https://greene-lab.gitbook.io/lab-website-template-docs/basics/citations). *Manubot will try it's best to pull from these sources automatically but it can make mistakes*.
- Resources: `resources/index.md` and create new posts in `_posts/` using the format `YYYY-MM-DD-resource-title.md`. You can also categorize resources by adding categories in the front matter of each post and make all sorts of embedddings in posts by leveraging [Jekyll SpaceShip](https://github.com/jeffreytse/jekyll-spaceship).

## Troubleshooting
If you encounter any issues while editing or deploying the website, please refer to the [Lab Website Template Documentation](https://greene-lab.gitbook.io/lab-website-template-docs) for basic documentation tips or check `_data/types.yaml` to check for known configurations. You can also open an issue or pull request in this repository for further assistance.

Known issues with local preview:
- GIT: Please ensure that [git](https://git-scm.com/install/) is installed and that it is configured to not have trailing spaces as there is a known issue with git adding trailing spaces in the wrong slashs when changing the environment type (Linux vs Windows) causes in entrypoint.sh to break.
    ```
    git config --global core.autocrlf input
    ```
    
- GIT: Please ensure that your git user name and email are configured to ensure that GitHub push and pull requests are correctly attributed. If you don't have them configured, it may not allow you to commit changes. You can do this by running the following commands in command line:
    ```
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

- Docker: If you encounter issues with Docker, ensure that Docker is properly installed and running on your machine prior to launching the file. You can refer to the [Docker installation guide](https://docs.docker.com/get-docker/) for assistance. You will also need an account (Free) on Docker to run the necessary images. If you encounter permission issues when running Docker commands, you may need to add your user to the Docker group or run commands with elevated privileges (e.g., using `sudo` on Linux).