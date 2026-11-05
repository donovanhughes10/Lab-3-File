Donovan Hughes — Portfolio

Personal portfolio site for Donovan Hughes: business administration student, college pitcher at Alvernia University, and owner of Like Ya Ask Services.

The whole site is one static file, index.html. There is no build step and no framework.

What's on the page
Hero: an interactive strike zone. Each of the nine cells is a highlight (Academic All-American, team captain, Student Athlete Award, crew leader, business owner, sales pitch competition, community service, Alvernia baseball, BotForge). Click a cell to see the details.
About: a short introduction.
Work history: a box-score style table of past and current jobs.
School: Alvernia University, County College of Morris, and Shore Regional High School.
Ventures: Like Ya Ask Services and BotForge.
Community: captaincy and volunteer work.
Contact: email link.
Run it locally

Open index.html in any browser. No server is needed.

To preview with a local server instead:

bash
python3 -m http.server 8000

Then visit http://localhost:8000.

Deploy with GitHub Pages
Push index.html and this README.md to the root of your repository.
In the repository, go to Settings → Pages.
Under Build and deployment, set Source to Deploy from a branch.
Choose your main branch and the / (root) folder, then click Save.
After a minute or two, the site is live at https://<your-username>.github.io/<repository-name>/.

If the repository is named <your-username>.github.io, the site is served at https://<your-username>.github.io/.

Edit your content

All content lives in index.html:

To change	Edit
Colors	The :root block at the top of the <style> section
Fonts	The Google Fonts <link> tag and the --display and --body variables
Work history	The <tbody> inside the #work section
Education	The three <article> blocks inside the #school section
Ventures	The two <article> blocks inside the #ventures section
Strike zone highlights	The items array in the <script> at the bottom, plus the matching button labels in the hero
Contact email	The mailto: link in the #contact section

Each strike zone button's position matches its entry in the items array, so keep the two lists in the same order.

Tech notes
Plain HTML, CSS, and a small amount of vanilla JavaScript.
Fonts: Archivo and Public Sans, loaded from Google Fonts. Without a connection the page falls back to system fonts.
Responsive down to phone widths.
Keyboard accessible, with visible focus outlines.
Respects the reduced-motion setting.
Contact

donovanhughes10@gmail.com
