# Fort Lewis College Nano Lab Wiki - Contribution Guide

This README serves as a guide for maintaining and updating the Fort Lewis College Nano Lab Wiki, with a specific focus on adding chemicals and SOPs to the repository.

## Project Structure

The wiki is organized with the following structure:

```
flcnanolab.github.io/
├── index.html           # Main entry point and application logic
├── pages/               # HTML page templates
│   ├── home.html        # Home page content
│   ├── sops.html        # SOP listing page
│   └── sop-template.html # Template for displaying individual SOPs
├── sops/                # SOP Markdown files
│   ├── photolith.md     # Photolithography SOP
│   └── new-sop.md       # (Example) New SOP
├── chemicals/           # Chemical information
│   └── chemicals.md     # Chemical inventory in markdown format
└── README.md            # This file
```

## How to Add a New Chemical

1. Open the `chemicals.md` file.
2. Add a new row to the appropriate table section following this format:

```markdown
| Name | Category | Location | Hazards | Datasheet | SDS |
|------|----------|----------|---------|-----------|-----|
| Your Chemical | Chemical Type | Storage Location | List of Hazards | [Datasheet](link-to-datasheet) | [SDS](link-to-sds) |
```

3. If your chemical belongs to a new category, add a new section with a heading:

```markdown
## New Category Name

| Name | Category | Location | Hazards | Datasheet | SDS |
|------|----------|----------|---------|-----------|-----|
| Your Chemical | Chemical Type | Storage Location | List of Hazards | [Datasheet](link-to-datasheet) | [SDS](link-to-sds) |
```

## How to Add a New SOP

### Create the SOP file:

1. Create a new Markdown file in the `sops` directory (e.g., `sops/new-procedure.md`)
2. Use the format shown in `photolith.md` as a template

### Add the SOP to the navigation:

1. Open `pages/sops.html`
2. Add a new row to the table:

```html
<tr>
  <td>Your SOP Title</td>
  <td><a href="#" onclick="loadSOP('Your SOP Title', 'sops/new-procedure.md')">View SOP</a></td>
</tr>
```

## SOP Markdown Format Guidelines

When creating SOPs, follow this structure:

1. **Header**: Include title, author, date, and adaptation source
   ```markdown
   Standard Operating Procedure (SOP)  
   Fort Lewis College  
   Senior Seminar 2024-2025

   **Author:** Your Name  
   **Updated:** Date

   ---

   ## Adapted From
   Original source
   ```

2. **Table of Contents**: List all sections with anchor links
   ```markdown
   ## Table of Contents

   1. [Equipment and Materials](#equipment-and-materials)
   2. [Startup Procedure](#startup-procedure)
   3. [Process Steps](#process-steps)
   ```

3. **Required Sections**:
   - Equipment and Materials
   - Startup Procedure
   - Process Steps
   - Shutdown Procedure
   - Parameters/Settings

4. **Tables**: Use markdown tables for process parameters
   ```markdown
   | Parameter | Value |
   |-----------|-------|
   | Temp (°C) | 110   |
   | Time (s)  | 60    |
   ```

5. **Math Equations**: Use LaTeX format between $$ symbols for equations
   ```markdown
   $$\text{Exposure Time [s]} = \frac{\text{Required Dose [mJ/cm²]}}{\text{Measured Intensity [mW/cm²]}}$$
   ```

## Site Navigation

The site uses client-side routing to navigate between sections:

- **Home**: General information about the lab
- **SOPs**: List of all standard operating procedures
- **Chemical Lists**: Inventory of all chemicals with safety information

## Deployment

After making changes:

1. Push your changes to the GitHub repository
2. The site will automatically update via GitHub Pages

For questions or issues, contact Sahra Genc, lab manager.
