# HRC Academic Website V1

1. Extract the ZIP. Upload the contents (not the enclosing folder) to ScienceOnFire/hrchamorro, branch main. Include hidden .github/workflows/hugo.yml; if missing, create that file separately using GitHub Add file > Create new file.
2. Settings > Pages > Source: GitHub Actions.
3. Actions > Publish academic website > Run workflow (main). Inspect the build log if it fails.
4. Open the URL shown by the deploy job.

Hugo extended 0.124.1 and LoveIt v0.2.11 are downloaded by the workflow. No local installation is required. These are older pinned versions chosen for compatibility; build has not been tested in this environment.

## Photo
Download your actual Scholar profile photo manually and upload it to static/images/profile.jpg. Change avatarURL in hugo.toml to images/profile.jpg. The current SVG is a neutral initials placeholder.

## Publications
Edit content/publications/index.md. Six sections are already present. The initial seven publication records come from EBSCO, KTH SweGRIDS and Rankless; not a complete Scholar export. Export all publications from your Scholar profile as BibTeX for a complete update. IEEE Access belongs in Other Journals, not IEEE Transactions. High Voltage may be placed in IET Journals if desired.

Sources:
- https://openurl.ebsco.com/results?bquery=AU+Chamorro%2C+Harold+R.
- https://penguin.eecs.kth.se/swegrids_projects/SP2
- https://www.rankless.org/authors/harold-r-chamorro

## CV
Upload your approved CV to static/pdf/CV.pdf and add a relative link in content/cv/index.md. No private or invented CV information is included.

## Maintenance
Edit Markdown files and commit. GitHub Actions rebuilds the site. Theme license is supplied by upstream at build time. No theme code is bundled.
