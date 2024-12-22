# Markdown to Google Docs Converter

A Python notebook that converts Markdown-formatted text into Google Docs while preserving formatting, structure, and special elements like checkboxes, mentions, and multi-level lists. The converter supports various Markdown elements including headings, bullet points, checkboxes, and mentions, making it ideal for converting meeting notes, documentation, and other structured text documents.

## Features

- Converts Markdown headings (H1-H3)
- Supports multi-level bullet points
- Handles checkbox lists
- Processes @mentions with special formatting
- Maintains document structure and indentation
- Supports footer formatting
- Batch processing of formatting requests

## Prerequisites

Before running this notebook, make sure you have:

- A Google account with access to Google Drive and Google Docs
- A Google Colab environment
- Required Python packages (automatically installed by the notebook)

## Dependencies

The notebook requires the following Python packages:
```
google-auth-oauthlib
google-auth-httplib2
google-api-python-client
markdown
```

## Setup Instructions

1. Open Google Colab (https://colab.research.google.com)
2. Create a new notebook or upload the existing .ipynb file
3. Mount your Google Drive when prompted
4. Run the authentication steps when prompted to allow access to your Google Docs

## Running in Google Colab

1. Open the notebook in Google Colab
2. Click on "Runtime" in the top menu
3. Select "Run all" to execute all cells, or run cells individually
4. When prompted, authorize the application to access your Google Drive and Docs
5. The script will create a new Google Doc with your converted Markdown content

## Usage

The notebook comes with a sample Markdown text for demonstration. To use with your own content:

1. Replace the `markdown_text` variable content with your own Markdown text
2. Run the notebook
3. The script will create a new Google Doc and provide you with a link to access it

## Example Input Format

```markdown
# Heading 1
## Heading 2
### Heading 3

* Bullet point
  * Nested bullet point
    * Deep nested bullet point

- [ ] Checkbox item
- [ ] Another checkbox item

Text with @mention
```

## Output

The script will:
1. Create a new Google Doc
2. Convert all Markdown formatting to appropriate Google Docs formatting
3. Provide a link to the created document
4. Apply all formatting including headings, bullets, checkboxes, and mentions

## Troubleshooting

If you encounter any issues:
- Make sure you're properly authenticated with Google
- Check that all required packages are installed
- Verify that your Markdown syntax is correct
- Ensure you have stable internet connection

## Limitations

- Currently supports up to H3 headings
- Requires manual authorization on first run
- Limited to 20 formatting requests per batch
- Some advanced Markdown features may not be supported