# i-restart Veterinary Learning

A discovery front end for the full i-restart veterinary training catalogue: 70 lessons, organised into 12 modules across data science, One Health and veterinary business.

Visitors can search lesson titles and learning outcomes, filter by curriculum or module, review lesson details, and continue to the existing Agrifood learning platform. Guidance explains how learners and educators can use the materials. V060 and V070 provide a more detailed example of the teaching packages.

## Run locally

This is a static website with no build step or package installation.

From this directory, run:

```sh
python -m http.server 8000
```

Open http://localhost:8000 in your browser. Serve the files over HTTP: opening index.html directly may prevent catalogue.json from loading.

## Files

- `index.html`: page content and accessible page structure
- `style.css`: responsive design
- `app.js`: search, filtering, lesson details and learner/educator guidance
- `catalogue.json`: all 70 lessons, outcomes, mapped delivery methods and platform links

To update the catalogue, edit the corresponding records in catalogue.json. Preserve unique lesson codes and check each platform URL. Lesson hours are intentionally omitted because the source mapping records them inconsistently.

## Hosting

Upload these four files together to any static web host, or configure GitHub Pages to serve the repository root. GitHub Pages is not enabled by this upload. No backend, platform password or other credentials are required by this website. Visitors sign in on the original learning platform when needed; this site does not collect or proxy their credentials.

The separate review preview is at https://i-restart-veterinary-learning.mark-bowenvet.chatgpt.site and currently requires its owner's ChatGPT sign-in. Updating this GitHub repository does not automatically update that preview.

## Source and attribution

The curriculum data comes from Veterinary_Activities_Content_Mapping (2).xlsx supplied by Mark Bowen and the veterinary catalogue at https://fields.learnskills.ie/course/index.php?categoryid=80 . Summaries adapt the learning outcomes for discovery. The programme context is i-restart, developed under the Erasmus+ Blueprint programme.

The V060/V070 example draws on teaching materials by the European Board of Veterinary Specialisation. The learning platform identifies its materials as CC BY-SA. Adapted catalogue text is shared on the same basis; see https://creativecommons.org/licenses/by-sa/4.0/ . Original resources remain on the learning platform with their own attribution and applicable licence. Fictional study examples are teaching exercises, not clinical evidence.

Delivery methods reflect the supplied mapping. Check the platform lesson for current arrangements and available files. This site does not synchronise platform changes or track learner completion.
