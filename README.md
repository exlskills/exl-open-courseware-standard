# EXL Open Courseware Standard (EOCS)

Welcome to the home of EOCS. This standard is currently a work-in-progress. To learn more, continue reading our README and star this repo on GitHub.

## About EXLskills

[EXLskills](https://exlskills.com) is on a mission to change education with an open-source online digital skills learning, certification, and peer-to-peer instruction platform that is committed to offering premium-quality courseware for 100% free via our open-source courseware methodology. Our courses are developed using the content in this repository and are then imported/pushed to [EXLskills.com](https://exlskills.com) with the [eocsutil](https://github.com/exlskills/eocsutil) tool. This process is 100% transparent, free, and open-source.

## File Structure
There are two main file structures for EOCS, the default and the optional file structure. The default file structure is designed for simple courses while the optional file structure is designed for courses that are more complex. The folder structures are shown below.

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

The optional file structure requires a different style of formatting as well as a separate folder for each vertical.

If the vertical contains more than 1 block, the standard format ```{index}_{name}.{ext}``` should be used to ensure that the ordering is correct on import/conversion. 

Inline code for verticals are setup with REPL, where each ```index.repl.yaml``` file is considered a block. The ```index.repl``` directory should contain a "source" directory for the inline code.

Use our [AP Java Course](https://github.com/exlskills/course-java-ap) as reference for the optional file structure.


## Index Files
Each course contains multiple index.yaml files that contain different information for each sublevel. The table below contains a brief description of each attribute and where it is located inside the folder structure. As shown below, each index.yaml file for the chapter, sequential, and vertical contain an attribute called ```url_name```. This attribute is a crucial component in the ```index.yaml``` file as these "url names" are used when updating the course. If no ```url_name``` is found (i.e. when you first import the course), a new ```url_name``` will be automatically created and will override the existing files (if any).

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
    <td>None</td>
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