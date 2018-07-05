# EXL Open Courseware Standard (EOCS)

Welcome to the home of EOCS. This standard is currently a work-in-progress. To learn more, continue reading our README and star this repo on GitHub.


**Course** <br />
&#8627; index.yaml<br />
&#160;&#160;&#160;&#160;**Chapters**<br />
&#160;&#160;&#160;&#160;&#8627; **Chapter Name (000_chaptername)**<br />
&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#8627; **Sequentials**<br />
&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#8627; **Sequential Name (000_sequentialname)**<br />
&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#8627; index.yaml<br />
&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;**Vertical Name (000_verticalname)**<br />

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
    <td>language</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>en</td>
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
  <tr>
    <td>grade_cutoffs</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>0.5</td>
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
    <td>display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>sequential url_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
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
    <td>display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>vertical url_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
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
    <td>display_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>problem url_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>html url_name</td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>IDE code </td>
    <td>markdown file</td>
    <td>Optional</td>
    <td>Generated from parent directory name</td>
  </tr>
  <tr>
    <td>grade weight</td>
    <td>index.yaml</td>
    <td>Required</td>
    <td>1</td>
  </tr>
</table>


**Custom Import Sequence:**

<table>
  <tr>
    <td>Import statement</td>
    <td>Target</td>
  </tr>
  <tr>
    <td>[//]: # (@import="../path/to/the/file.md") </td>
    <td>file</td>
  </tr>
  <tr>
    <td>[//]: # (@import="file://../path/to/the/file.md") </td>
    <td>file</td>
  </tr>
  <tr>
    <td>[//]: # (@import="exlcode://../path/to/the/file.md")</td>
    <td>exlcode</td>
  </tr>
</table>


<table>
  <tr>
    <td>Symbol</td>
    <td>Directory</td>
  </tr>
  <tr>
    <td>./</td>
    <td>Current Directory</td>
  </tr>
  <tr>
    <td>../</td>
    <td>Parent Directory</td>
  </tr>
  <tr>
    <td>None</td>
    <td>Course Directory</td>
  </tr>
</table>



