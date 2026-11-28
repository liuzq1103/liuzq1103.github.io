# Zhi-Qiang Liu — Personal Academic Website

Bilingual personal academic portal, published with GitHub Pages.

**Website:** https://liuzq1103.github.io/

## Site structure

- \`index.html\` — bilingual homepage, research interests, featured work, selected publications, resource entry points, and software projects.
- \`publications.html\` — searchable and filterable publication archive.
- \`resources.html\` — categorized research-resource directory.
- \`cv.html\` — browser-based viewer and download link for the PDF CV.
- \`style.css\` — responsive visual system.
- \`data/resources.json\` — resource catalog data; add new database links here without changing page layout.
- \`assets/people/liuzq.jpeg\` — profile photo.
- \`assets/people/liuzq_cv.pdf\` — source CV PDF.
- \`assets/news/NN_GraphicalAbstract.jpg\` — featured publication graphic.

## Adding a resource

Edit \`data/resources.json\` and append an item to the appropriate category's \`items\` array.

Example item:

\`\`\`json
{
  "title": "Database name",
  "url": "https://official-database.example.org/",
  "description": {
    "zh": "数据库用途与主要内容。",
    "en": "A short description of the database and its contents."
  },
  "type": "Database",
  "species": ["human", "mouse"],
  "tags": ["single-cell", "brain"],
  "updated": "2026-11-28"
}
\`\`\`

Use stable HTTPS links and prefer official database or project pages. The resource page renders entries automatically and supports keyword search.

## Updating publications

Publication metadata and links are maintained in \`publications.html\`. Verify author order, publication year, DOI, and author-contribution notes against the publisher or PubMed record before adding or editing an entry.

The public publication archive is an online-indexed list and should be cross-checked against the current CV before being treated as a complete academic bibliography.

## Updating the CV

Replace \`assets/people/liuzq_cv.pdf\` with the reviewed PDF while keeping the filename unchanged. The CV page embeds this file and provides a direct download link.
