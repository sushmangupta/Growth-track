# File structure and management

The growth track is a university of knowledge that primarily focuses on upskilling individuals associated with Shopware, including developers, partners, agencies, newcomers, and more. It is geared towards strategic and structured skill development, with a timeline for completion. It offers both certified and non-certified programs. Resources in the academy include learning paths, courses, and learning units.

Conversely, the monitoring track promarily upholds Knowledge Drop-Ins. It provides quick technology insights such as video snippets, blog posts, event updates, release notes, and podcasts.

Currently, the emphasis is on defining the Growth track.

- *Learning path* : A defined route towards a specific learning goal, like becoming a Shopware App Developer, encompassing all necessary knowledge, mindset, and skill sets. A Learning Path typically comprises multiple courses and is completed over days or weeks.

- *Course* : A significant milestone within a learning path. Courses may belong to multiple paths, especially fundamental ones. The aim is to acquire skills and knowledge required for a specific goal within a broader learning journey. For instance, creating a simple app could be a course, while mastering advanced techniques could be another course within the same learning journey. A course consists of multiple learning units and typically takes hours to days to complete.

- *Learning Unit / Bit* : AThe smallest component of the learning journey, focusing on transferring specific thoughts, ideas, or skills necessary to succeed in a course and eventually a full learning path. For example, an overview of Shopware's folder structure could be a learning unit, while details of each folder constitute additional units. A learning unit should be concise, typically no longer than 25 minutes, and may include text, videos, or practice exercises. External learning units may also be provided, possibly associated with specific courses.

This learning unit will mostly accomodate 3 types of assets:

- Text files in `.md` format
- Screenshots in `.png` format
- Video shots in `.wmv`/... format

## Naming conventions

Maintaining a well-organized repository for all documentation assets, including images, videos, and files, is crucial. This section provides an overview of how assets are represented, managed, and the naming conventions that are adhered to.

::: info
For the creation of a visual representation, use the [figma diagram library](https://www.figma.com/file/6rki2S5MhWAnfV9vy0XcHN/Diagrams-documentation?type=design&mode=design&t=w97uZM4w6FDyQ5r2-0)
:::

### Asset specifications

| Image attributes | Specification | Notes|
|------------------|---------------|---------|
| File type| Only .png, .svg| Use a lossless image format for screenshots (i.e., PNG) and vector format (i.e., SVG) for drawings (diagram, chart, logos, ...).|
|Folder size | ? | A learning unit can hold text, images and videos. Place all these in the strcuture mentioned below |
|File name | Only use letters and hyphens | Use the naming convention documented below in naming conventions for different assets.|
|Image size | Width: max 768px, Height: max 576px | This is automatically taken care by the inbuilt functions in our docs.|
|Aspect ratio | 4:3 | This is automatically taken care by the inbuilt functions in our docs. |
|Copyright| - |Determine if an image or diagram is protected by copyright. If it is, you must obtain permission and acknowledge credit.|
|Personal identifiable information (PII) | - | Make sure to mask, modify, or remove any PII such as passwords, logins, account details, or other information that could compromise security.|
|Alt tags| `![Alt](/path/to/img.jpg “image title”)` | Make sure to include alt text for every image. The text is used in situations where the image isn’t visible and image SEOs.|
|Borders|-|No borders are added to the images|

### File structure

```text
└── Learning path
    └── Course1
        └── Learning unit
            ├── Text
            ├── Imges
            └── Videos
    └── Course2
        └── Learning unit
            ├── Text
            ├── Imges
            └── Videos
    └── Course3
        └── Learning unit1
            ├── Text
            ├── Imges
            └── Videos
        └── Learning unit2
            ├── Text
            ├── Imges
            └── Videos
```

### Naming conventions

* Every learning resource must have a unique name.

|Learning resource|Naming convention|
|-----------------|-----------------|
|Learning unit|<LU-NUMBER>-<meaningfulName.md>|
|Course|<CO-NUMBER>-<meaningfulName.md>|
|Learning path|<LP-NUMBER>-<meaningfulName.md>|

## Screenshots

### Considerations for Diagrams

Consider creating screenshots to :

* Provide an example of a visualization
* Show panels populated with query and settings
* Show configurations and settings
* Emphasize a new feature
* Limit the contents of an image to the relevant portion. Do not include distracting or unnecessary content and whitespace.

### Aspects for Capturing Screenshots

* If the screenshot shows a desktop application interface, you must use the latest OS version supported by the solution to take the screenshot.
* The screenshot must be in focus and show an active window, wizard or dialog box.
* Avoid both horizontal and vertical scroll bars whenever possible.
* The screenshot must show real-world data or at least data that is close to realistic use cases.
* All screenshots you take must be consistent with each other.
* Screenshots can be taken using GIMP, Snipping tools, or any tool you have already worked on.
* Do not use screenshots for Code samples (show code samples in codeblocks).
* Do not take screenshots for a page that is likely to change frequently.

## Others

* The video is to be placed at the top followed by text, images and code snippets.

* Store all the media in the assets directory specific to each learning path.

* If you add screenshot to illustrate items in a list (typically, steps in a procedure), align them accordingly:
    * If there is only one image that illustrates the entire procedure, place the image at the end of the procedure or align it with the lead-in paragraph.
    * If you need to provide an image for each step in the procedure, place each image at the end of each step it follows.
    * The image names can be serialized if multiple images are under the same topic. For example,

* An introductory sentence should precede most screenshots.
