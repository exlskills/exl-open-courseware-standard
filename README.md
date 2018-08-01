# EXL Open Courseware Standard (EOCS)

Welcome to the home of EOCS. This standard is currently a work-in-progress. To learn more, continue reading our README and star this repo on GitHub.

**File Structures**<br/>

Default:

```
course
├── index.yaml
└── chapter_name (00_chaptername)
    └── sequential_name (00_sequentialname)
        ├── index.yaml
        └── vertical_name(00_verticalname)
```

Optional:

```
course
├── index.yaml
└── chapter_name (00_chaptername)
    └── sequential_name (00_sequentialname)
        ├── index.yaml
        └── vertical_name(00_verticalname)
            ├── index.yaml
            └── index.md
```
<br/>

**Course:**

<table>
  <tr>
    <td>Attribute</td>
    <td>Location</td>
    <td>Optional/Required</td>
    <td>Default</td>
  </tr>
  <tr>
    <td>advanced_modules</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>cert_html_view_enabled</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>true</td>
  </tr>
  <tr>
    <td>chapter url_name</td>
    <td>markdown file</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>course</td>
    <td>markdown file</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>course url_name</td>
    <td>markdown file</td>
    <td>Required</td>
    <td>"course"</td>
  </tr>
  <tr>
    <td>course_image</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>enrollment_start</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>grade_cutoffs</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>0.5</td>
  </tr>
  <tr>
    <td>language</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>en</td>
  </tr>
  <tr>
    <td>org</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>None</td>
  </tr>
  <tr>
    <td>self_paced</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>true</td>
  </tr>
  <tr>
    <td>start</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>wiki slug</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>
</table>


**Chapter:**

<table>
  <tr>
    <td>Attribute</td>
    <td>Location</td>
    <td>Optional/Required</td>
    <td>Default</td>
  </tr>
  <tr>
    <td>chapter display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>sequential url_name</td>
    <td>markdown file</td>
    <td>Required</td>
    <td>None</td>
  </tr>
</table>


**Sequential:**

<table>
  <tr>
    <td>Attribute</td>
    <td>Location</td>
    <td>Optional/Required</td>
    <td>Default</td>
  </tr>
  <tr>
    <td>sequential display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>vertical url_name</td>
    <td>markdown file</td>
    <td>Required</td>
    <td>None</td>
  </tr>
</table>


**Vertical:**

<table>
  <tr>
    <td>Attribute</td>
    <td>Location</td>
    <td>Optional/Required</td>
    <td>Default</td>
  </tr>
  <tr>
    <td>vertical display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>grade_weight</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>1</td>
  </tr>