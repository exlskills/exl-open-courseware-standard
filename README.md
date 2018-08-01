# EXL Open Courseware Standard (EOCS)

Welcome to the home of EOCS. This standard is currently a work-in-progress. To learn more, continue reading our README and star this repo on GitHub.

**File Structure**<br/>

Default:

```
course
├── index.yaml
└── chapter_name (00_chaptername)
    ├── index.yaml
    └── sequential_name (00_sequentialname)
        ├── index.yaml
        └── vertical_name.md (00_verticalname)
```

Optional:

```
course
├── index.yaml
└── chapter_name (00_chaptername)
    ├── index.yaml
    └── sequential_name (00_sequentialname)
        ├── index.yaml
        └── vertical_name (00_verticalname)
            ├── index.yaml
            ├── index.md
            ├── index.repl
            └── index.repl.yaml
```
Formatting verticals:

If the vertical contains more than 1 block, the standard format ```{index}_{name}.{ext}``` should be used to ensure that the ordering is correct on import/conversion. 

Setting up REPL:

Inline code for verticals are setup with REPL, where each ```index.repl.yaml``` file is considered a block. The ```index.repl``` folder should contain a "source" directory and a "test" directory for the inline code.

<br />

**Course:**

<table>
  <tr>
    <td>Attribute</td>
    <td>Location</td>
    <td>Optional/Required</td>
    <td>Default</td>
  </tr>
  <tr>
    <td>course</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>
  <tr>
    <td>course url_name</td>
    <td>index.yaml</td>
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
    <td>index.yaml</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
    <tr>
    <td>est_minutes</td>
    <td>index.yaml</td>
    <td>Optional</td>
    <td>None</td>
  </tr>
  <tr>
    <td>language</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>en</td>
  </tr>
  <tr>
    <td>org</td>
    <td>index.yaml</td>
    <td>Optional</td>
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
    <td>index.yaml</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>chapter url_name</td>
    <td>index.yaml</td>
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
    <td>format</td>
    <td>index.yaml</td>
    <td>Optional</td>
    <td>Homework</td>
  </tr>
  <tr>
    <td>graded</td>
    <td>index.yaml</td>
    <td>Optional</td>
    <td>true</td>
  </tr>
  <tr>
    <td>sequential display_name</td>
    <td>index.yaml</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>sequential url_name</td>
    <td>index.yaml</td>
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
    <td>api_version</td>
    <td>index.repl</td>
    <td>Optional</td>
    <td>1</td>
  </tr>
  <tr>
    <td>environment</td>
    <td>index.repl</td>
    <td>Optional</td>
    <td>None</td>
  </tr>
  <tr>
    <td>height</td>
    <td>index.repl</td>
    <td>Optional</td>
    <td>500px</td>
  </tr>
  <tr>
    <td>src_path</td>
    <td>index.repl</td>
    <td>Optional</td>
    <td>None</td>
  </tr>
    <tr>
    <td>test_path</td>
    <td>index.repl</td>
    <td>Optional</td>
    <td>None</td>
  </tr>
  <tr>
    <td>vertical display_name</td>
    <td>index.yaml</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>vertical url_name</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>None</td>
  </tr>