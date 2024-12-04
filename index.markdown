---
layout: default
title:  "An Overview on Jekyll"
categories: jekyll update
---

## Welcome

Welcome to my page! Here, I will explain how I used the **Jekyll framework** to create and host a simple webpage, explaining the steps I used, the challenges I encountered, and how I resolved them.

---

### Installing Jekyll

1. **Installation**:
To begin, you need to have Ruby installed on your computer. Once Ruby is installed, open your terminal or command prompt and use Ruby's package manager, gem, to install Jekyll and Bundler.
   - I installed Ruby using the official [Ruby Installer](https://rubyinstaller.org/) for Windows. 
   - During installation, I selected the option to include DevKit, which is necessary for compiling native extensions for some Ruby gems.

2. **Bundler and Jekyll**:
   - Using the terminal, I installed Bundler and Jekyll with the following commands:
     ```bash
     gem install bundler
     gem install jekyll
     ```

     --> some tips:
     to verify the installation I typed **jekyll -v** in the terminal. This helped me verify the installed version on my machine. 

3. **Created a New Site**:
   - To initialized a new Jekyll site I typed:
     ```bash
     jekyll new my-site
     cd my-site
     ```
   This sets up a ready-to-use Jekyll project in the my-site directory. To preview the site locally, I navigated to the my-site directory and executed **bundle exec jekyll serve**.

4. **Testing Locally**:
   - To preview my site, I ran the following command on my terminal:
     ```bash
     bundle exec jekyll serve
     ```
   - The site was accessible at `http://127.0.0.1:4000` on my browser.

---

### How I Built This Page

1. **Site Structure**:
   - Jekyll uses a combination of Markdown files and layouts. 
   - I edited the `_posts` directory to include this page and added my content to this Markdown file:
     ```
     _posts/2024-12-02-building-with-jekyll.md
     ```
   - Jekyll requires the filename format `YEAR-MONTH-DAY-title.md` to generate posts correctly.

2. **Edited Layouts**:
   - The overall structure of the page is controlled by the `_layouts` directory. I customized the `default.html` layout to improve styling and structure.

3. **Custom CSS**:
   - I added styles directly in the `_includes` or `_sass` directories for a clean look.

4. **Hosted on GitHub Pages**:
   - After completing the design and content updates, I pushed the project to a GitHub repository and enabled GitHub Pages in the repository settings.

---

### Challenges and Solutions

1. **Ruby Installation Issues**:
   - **Challenge**: Ruby installation on Windows required additional steps for compatibility.
   - **Solution**: I used the RubyInstaller with DevKit to simplify the process.

2. **Understanding Folder Structure**:
   - **Challenge**: Initially, it was unclear to me how `_posts`, `_layouts`, and `_config.yml` interacted and what their purposes were. The documentation for each folder was new and I had to read through each to see what their roles were.
   - **Solution**: I referred to the [Jekyll Documentation](https://jekyllrb.com/docs/) to understand how Jekyll generates static content and what the importance was for each file/folder.

3. **Deployment Difficulties**:
   - **Challenge**: Configuring GitHub Pages to host the Jekyll site required adjustments to `_config.yml`, as well uploading it to Github Pages was new for me as I have never used that feature before for deployment.
   - **Solution**: I ensured the `baseurl` and `url` fields in `_config.yml` were correctly set to match my GitHub repository and I read a tutorial for Github Pages to make sure the procedure was done correctly for deployment.

---

### Closing Remarks

After experimenting with this framework, using Jekyll was a good experience. Its combination of simple and flexibility makes it an easy choice for hosting static sites. The biggest learning takeaways for me was understanding how Markdown, layouts, and configuration files work to help generate a clean, simple, easy and responsive webpage.

To learn more, you can read the [Jekyll Documentation](https://jekyllrb.com/docs/) for more tips and tricks!
