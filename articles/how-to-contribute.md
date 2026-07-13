One of the primary advantages of utilizing plain Markdown files over closed databases is how easily anyone can contribute to or edit the knowledge base.

To add a new question or modify an existing response, simply follow these basic steps:

#### Step 1: Create or Edit the Markdown File
Navigate to the `articles/` directory inside the repository.
- To **edit** an article, open the corresponding `.md` file and click the pencil icon (Edit).
- To **add** a new entry, create a file using a descriptive name written entirely in lowercase (e.g., `my-new-topic.md`).

Write your content using traditional Markdown. You can format your text with bold tags (`**text**`), headings (`#### Subheading`), or lists (`- item`) as you see fit.

#### Step 2: Update the Search Index
For your new topic to become searchable for users on the homepage, open the `index.json` file in the root folder and append a new object to the array:

```json
{
  "id": "my-new-topic",
  "discipline": "category",
  "title": "Your new question title here?",
  "abstract": "A short summary displaying on the homepage card.",
  "tags": ["keywords"]
}
```

*Ensure that the `id` field in the JSON registry matches your `.md` file name **exactly** (always use lowercase).*
