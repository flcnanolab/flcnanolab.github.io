# Fort Lewis College Nano Lab Wiki - Comprehensive Contribution Guide

This README serves as a complete guide for maintaining and updating the Fort Lewis College Nano Lab Wiki. It covers how to add chemicals, SOPs, and new pages to the site.

## Website Overview

The FLC Nano Lab Wiki is a browser-based information repository for lab procedures, chemical inventories, research papers, and projects. The site uses a combination of HTML and Markdown files, with GitHub Pages for hosting.

## Project Structure

```
flcnanolab.github.io/
├── index.html           # Main entry point with navigation and application logic
├── index.md             # Home page content in Markdown
├── projects.md          # Projects page content in Markdown
├── papers.md            # Publications page content in Markdown
├── sops/                # SOP Markdown files
│   ├── photolith.md     # Photolithography SOP
│   └── [other-sops].md
├── chemicals/           # Chemical information
│   └── chemicals.md     # Chemical inventory in Markdown format
├── templates/           # HTML templates for dynamic content
│   ├── sops.html        # SOP listing page
│   └── sop-template.html # Template for displaying individual SOPs
└── assets/              # Static assets like images, PDFs, etc.
    ├── images/
    └── pdfs/
```

## How to Add or Update Content

### Adding Chemicals to the Inventory

1. **Navigate to the chemicals file**:
   - Go to `chemicals/chemicals.md` in the repository

2. **Edit the file**:
   - Click the pencil icon to enter edit mode
   - Find the appropriate section or create a new one
   
3. **Add your chemical entry**:
   ```markdown
   ## [Category Name]
   
   | Name | Category | Location | Hazards | Datasheet | SDS |
   |------|----------|----------|---------|-----------|-----|
   | New Chemical | Chemical Type | Storage Location | Hazard 1, Hazard 2 | [Datasheet](URL) | [SDS](URL) |
   ```

4. **Example**:
   ```markdown
   ## Etchants
   
   | Name | Category | Location | Hazards | Datasheet | SDS |
   |------|----------|----------|---------|-----------|-----|
   | Aluminum Etchant Type A | Etchant | Acid Cabinet | Corrosive, Toxic | [Datasheet](https://www.sigmaaldrich.com/specification-sheets/262/381/901539-BULK.pdf) | [SDS](https://www.sigmaaldrich.com/US/en/sds/aldrich/901539) |
   ```

5. **Commit your changes**:
   - Add a descriptive commit message (e.g., "Added Aluminum Etchant Type A to chemicals inventory")
   - Click "Commit changes"

### Adding a New SOP

1. **Create a new SOP file**:
   - Navigate to the `sops/` folder
   - Click "Add file" > "Create new file"
   - Name your file (e.g., `etching.md`)
   
2. **Format your SOP using this template**:
   ```markdown
   Standard Operating Procedure (SOP)  
   Fort Lewis College  
   Senior Seminar 2024-2025

   **Author:** Your Name  
   **Updated:** Date

   ---

   ## Adapted From

   [Source of procedure, if applicable]

   ---

   ## Notes

   [Brief description of the SOP]

   ---

   ## Table of Contents

   1. [Equipment and Materials](#equipment-and-materials)
   2. [Startup Procedure](#startup-procedure)
   3. [Process Steps](#process-steps)
   [etc.]

   ---

   ## Equipment and Materials

   [List equipment and materials]

   ---

   ## Startup Procedure

   [Detailed startup steps]

   [Continued sections...]
   ```

3. **Update the SOP listing page**:
   - Navigate to `templates/sops.html`
   - Edit the file and add your SOP to the table:
   ```html
   <tr>
     <td>Your SOP Title</td>
     <td><a href="#" onclick="loadSOP('Your SOP Title', 'sops/your-file.md')">View SOP</a></td>
   </tr>
   ```
   
4. **Commit your changes** for both the new SOP file and the updated listing page

### Adding or Updating Major Pages (Projects/Papers/Home)

1. **Navigate to the file**:
   - For the home page: `index.md`
   - For the projects page: `projects.md`
   - For the papers page: `papers.md`
   
2. **Edit the file using Markdown formatting**:
   - Click the pencil icon to edit
   - Update or add content following the existing format
   
3. **For projects**, use this structure for each project:
   ```markdown
   ### Project Name

   ![Project Image](/assets/images/project-image.jpg)

   **Principal Investigator:** Dr. Name  
   **Students:** Student Names  
   **Funding:** Funding Source

   **Description:**  
   Project description goes here.

   **Key Research Areas:**
   - Area 1
   - Area 2
   - Area 3
   ```

4. **For papers**, use this structure:
   ```markdown
   ### Year
   1. **Paper Title**  
      Authors: Author Names  
      *Journal Name*, Volume(Issue), Pages.  
      [DOI: xxx.xxxx/xxxxx](https://doi.org/)  
      [PDF Download](/assets/pdfs/filename.pdf)
   ```
   
5. **Commit your changes** with a descriptive message

## Markdown Formatting Guide

For those new to Markdown, here's a quick reference:

### Basic Formatting

```markdown
# Level 1 Heading (largest)
## Level 2 Heading
### Level 3 Heading

**Bold text**
*Italic text*

[Link text](URL)
![Image alt text](image-url.jpg)

- Bullet point
- Another bullet point
  - Indented bullet point

1. Numbered item
2. Another numbered item
```

### Tables

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Cell 1   | Cell 2   | Cell 3   |
| Cell 4   | Cell 5   | Cell 6   |
```

### Code Blocks

````markdown
```
Code goes here
```
````

## GitHub Best Practices

### Making Changes

1. **Always preview changes** before committing
2. **Use clear commit messages** that explain what you changed
3. **Make one logical change per commit** rather than multiple unrelated changes
4. **Check your work** on the live site after committing

### Adding Files & Images

1. **Images**:
   - Add images to the `assets/images/` directory
   - Reference them in Markdown: `![Description](/assets/images/filename.jpg)`
   
2. **PDFs and other documents**:
   - Add them to the `assets/pdfs/` directory
   - Link to them: `[Document Name](/assets/pdfs/filename.pdf)`

## Website Deployment

After committing changes:

1. GitHub automatically rebuilds the site (typically within 1-2 minutes)
2. Visit the live site at [flcnanolab.github.io](https://flcnanolab.github.io) to verify your changes
3. If changes don't appear, try clearing your browser cache or waiting a few more minutes

## Getting Help

If you encounter any issues while updating the website:

- Review this README and the [Markdown Guide](https://www.markdownguide.org)
- Check GitHub's documentation at [docs.github.com](https://docs.github.com)
- Contact the lab webmaster: [email@fortlewis.edu](mailto:lascheer@fortlewis.edu)

Thank you for contributing to the FLC Nano Lab Wiki!
`
