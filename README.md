# Live Link to [KawShon DEV's Guide to the Galaxy](https://jkawahara.github.io)
### 1. Why / Background
  * KawShon DEV's Guide to the Galaxy is a static website for presenting a portfolio of projects and blogging posts.
 ### 2. What / Objectives / User Stories
  * This project development, from design through deployment of the application, used Jekyll as a static site generator using Markdown, Liquid, Front Matter, HTML, CSS on the client-side along with the Architect theme:
  * User Stories, by categorization:
    * Set up web application framework
    * Set up View templates
      * About Me
      * Blog Posts
      * Software Apps Portfolio
      * Product Roadmap Portfolio
      * Contact Me
 ### 3. How / Design Description
  * The scope of the project fits ell into [Agile methodology with Scrum and Kanban frameworks](https://en.wikipedia.org/wiki/Agile_software_development). Due to limited scope and non-group assignment, GitHub's built-in tools were not used to support project execution:
    * Projects: Kanban board for documenting user stories and overall progress
    * Issues: Issue tracking for user stories, features and bug report
  * Functionality:
    * Design Description
      * Install The Architect theme as starting basis for pages
      * View Setup (*.html, _layouts, _includes, _posts)
        * For each page (*.html), use Front Matter to predefine variables (layout, title, heading) and inherit specific layout
          * _layouts: index, software, product, blog, contact.html inherit from page, post.html, which in turn, inherit from default.html
          * _includes: links, navigation.html included in default.html 
          * _data: navigation, portfolio-software, portfolio-tech, sidebar.yml custom data is accessed by links, navigation, index.html
        * For each page (*.html), use Liquid to process templates:
          * {{ variable }} to output content
          * {% logic %} to perform logic statements
        * For contact.html, use action attribute within form element to connect to Formspree email contact forms
        * About Me ![aboutme.png](/assets/images/aboutme.png "aboutme")
        * Software Apps ![software.png](/assets/images/software.png "softwareapps")
        * Product Roadmap ![product.png](/assets/images/product.png "productroadmap")
        * Blog Posts ![blogs.png](/assets/images/blogs.png "blogposts")
        * Contact Me ![contactme.png](/assets/images/contactme.png "contactme")
  * Prerequisites for Development:
    * MacBook Air (Intel Core i7, 2.2 GHz, 1 Processor, 2 Cores, 8GB)
    * 64 bit operating system 
    * git version 2.18.0
    * Visual Studio Code Version 1.29.1
    * [GitHub Repo](https://github.com/jkawahara/jkawahara.github.io)
    * Chrome Version 70.0.3538.110 (Official Build) (64-bit)
  * Built with:
    * Client-side [Jekyll](https://jekyllrb.com/):
      * [Markdown](https://daringfireball.net/projects/markdown/)
      * [Liquid](https://shopify.github.io/liquid/)
      * [Front Matter](https://jekyllrb.com/docs/front-matter/)
      * HTML, CSS
      * [The Architech theme](https://github.com/pages-themes/architect)
    * Cloud:
      * [GitHub Pages](https://pages.github.com/)
      * [Formspree](https://formspree.io/)
  * Installing:
    * For further development or use of this application, clone or download application files from GitHub, which is organized into the following directory structure:
      * /kawshon (application root directory level)
        * /_data
          * navigation.yml
          * portfolio.yml
          * sidebar.yml
        * /_drafts (YEAR-MONTH-DAY-title.MARKUP)
        * /_includes
          * links.html
          * navigation.html
        * /_layouts
          * default.html
          * page.html
          * post.html
        * /_posts (YEAR-MONTH-DAY-title.MARKUP)
        * /_site (generated site)
        * /_assets
          * /css
            * print.css
            * pygment_trac.css
            * stylesheet.css
          * /images
          * /js
        * _config.yml
        * .gitignore
        * aboutme.html
        * blog.html
        * contact.html
        * Gemfile
        * Gemfile.lock
        * index.html
        * LICENSE
        * jekyll-architect-theme.gempspec
        * README.md
  * Running the tests:
    * Unit testing & integration testing was informally executed
  * Deployment:
    * Deployed on [GitHub Pages](https://jkawahara.github.io)
 ## Versioning
  * For the versions available, see the tags on this repository.
 ## Authors
  * John Kawahara.
  * N/A- See also the list of contributors who participated in this project.
 ## License
  * This project is licensed under the [MIT License](LICENSE).
 ## Acknowledgments
  * Thanks to David Hallinan, Hannah Bowers and Glo Austin for their guidance and support.
