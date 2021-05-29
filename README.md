
# PeterLu.org jekyll source repository

This repository houses the jekyll source files for PeterLu.org. The static output is housed at the `peterlu.github.io` repository. 

A separate output repository is needed because the site uses jekyll plugins that aren't supported by github pages. The plugins include:
- jekyll-scholar for bibliography management
- jekyll-polyglot (for multiple language support).

## Front page

The front matter of index.md determines:
- The pages displayed in the carousel. Typically these are the research topic pages, identified by the `id` in their front matter, but any page wit hand `id` and a `thumbnail` is supported
- A link to a soundcloud playlist for the "Broadcast Media" player
- The publications, listed by their id in the publications.bib file in the _bibliography folder
- Broadcast Media references, listed by their id in the broadcast_media.bib file in the _bibliography folder
- Print Media references, listed by their id in the print_media.bib file in the _bibliography folder

## Photo

The front mater of photo.md determines the galleries displayed there. The filenames refer both to the large images in images/large, and the thumbnails in images/thumbs. (They must match.)

## Video

The frontmatter of video.md lists youtube videos by their id, not the full url. (For example, with "https://www.youtube.com/watch?v=6AJx8IVcL_c", use everything after the "?v=", or "6AJx8IVcL_c".)

The videos also have an optional title attribute, which appears as text over the video thumbnail.

## Media Coverage

The frontmatter of mediacoverage/index.md just contains a soundcloud playlist link for the broadcast meda player. The list of references on this pages is the full contents of broadcast_media.bib and print_media.bib in the _bibliography folder. Reference formatting is determined by science-mediacoverage-plu.csl in the _data folder. The .csl file is based on the Science csl, but modified to meet the needs of this site.

## Publications

The front matter of publications/index.md prints the full contents of publications.bib in the _bibliography folder. Reference formatting is determined by science-plu.csl in the _data folder. The .csl file is based on the Science csl, but modified to meet the needs of this site.

## Research

The frontmatter of research.md lists the topics shown on this page, in order, by the id in their page's front matter. The areas listed are for the sorting (filtering) links at the top of the page. Each area has an id that matches the areas listed in the frontmatter of topics. This area id also determines the translation provided in locale.yml files.

## Research Topics

The front matter of each research topic has many optional types of content, many mirroring the approaches above. They include:
- **title:**
- **lang:** (for example, "en" for English. Translations are supported by the jekyll-polyglot plugin, with fallbacks to English. The translations should be provided in the coresponding folder in the _data folder. For example, French translations go in _data/fr.)
- **id:** a unique identifier for this topic but the same for translations. Used to refer to this topic on the front page and research page.
- **permalink:** unique to this topic, but the same for translations.
- **areas:** used for the sorting links on the research page
- **thumbnail:** The filename for a square thumbnail, 300px x 300px, in teh images/topic_thumbs folder.
- **youtube_single:** Just the id (everything after the "?v=") of a video's URL.
- **youtube_playlist:** Just the id (everything between the "?list=" and "&v=", if present) of a playlist's URL.
- **soundcloud:** The URL of a soundcloud playlist to embed in a player on the page.
- **images:** Each with a filename of a file in images/large folder, and matching file in images/small, and an optional caption.
- **publications:** Id's from publications.bib
- **broadcast_media:** Id's from broadcast_media.bib
- **print_media:** Id's from print_media.bib
- **links:** In HTML form.

The text content of the page, and any other custom markdown or HTML, goes after the frontmatter.

## Translations
When providing a translation for a topic, only alter the contents (not the labels) for these:
- title
- lang 
- description
- body text after the frontmatter

DO NOT alter:
- permalink
- id
- areas
- or any media or publications attributes

Site-wide translations for snippets of text are provided in _data/locale.yml for English, and the locale.yml files in each corresponding language folder in _data (e.g. _data/fr/locale.yml)
