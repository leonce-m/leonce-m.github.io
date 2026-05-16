# CV Page Images

The `/cv/` page displays rendered JPEG pages from `cv_leonce_mollerus.pdf` instead of embedding the PDF viewer directly. This gives more consistent layout control across browsers.

Regenerate the page images after updating the PDF:

```sh
mkdir -p assets/cv/pages
pdftoppm -jpeg -r 180 -jpegopt quality=92 assets/cv/cv_leonce_mollerus.pdf assets/cv/pages/cv-page
```

This creates files like:

```text
assets/cv/pages/cv-page-1.jpg
assets/cv/pages/cv-page-2.jpg
```

The `/cv/` page automatically renders every file in `assets/cv/pages/` in filename order, so the page count does not need to be updated manually.
