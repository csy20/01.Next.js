# HTML (HyperText Markup Language) - The Structure

## What is HTML?

HTML is like the **skeleton** of a website. Just like how your body has bones that give it structure, HTML gives structure to web pages. It tells the browser what content to display and how to organize it.

Think of HTML as a way to **label** different parts of your content so the browser knows what each part is supposed to be.

## Basic HTML Structure

Every HTML page follows this basic pattern:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <!-- Your content goes here -->
</body>
</html>
```

- `<!DOCTYPE html>` - Tells the browser this is an HTML5 document
- `<html>` - The root container for everything
- `<head>` - Information about the page (not visible to users)
- `<body>` - The visible content of the page

## Common HTML Tags Explained

### 1. `<div>` - The Generic Container
**What it is:** A generic box that groups other elements together.

**When to use:** When you need to group elements or create sections.

```html
<div>
    <h1>Welcome to my website</h1>
    <p>This is some content inside a div.</p>
</div>
```

**Think of it as:** A cardboard box that holds other things together.

### 2. `<span>` - The Inline Container
**What it is:** Like `<div>`, but for small pieces of text within a line.

**When to use:** When you want to style just part of a sentence.

```html
<p>This is a normal sentence with <span>highlighted text</span> in the middle.</p>
```

**Think of it as:** A highlighter that marks specific words.

### 3. `<h1>` to `<h6>` - Headings
**What they are:** Different sizes of titles and subtitles.

**When to use:** For page titles, section headers, and organizing content hierarchy.

```html
<h1>Main Title (Biggest)</h1>
<h2>Section Title</h2>
<h3>Subsection Title</h3>
<h4>Smaller Heading</h4>
<h5>Even Smaller</h5>
<h6>Smallest Heading</h6>
```

**Think of them as:** Like chapter titles in a book - `<h1>` is the book title, `<h2>` is chapter titles, etc.

### 4. `<p>` - Paragraph
**What it is:** A block of text, like a paragraph in a book.

**When to use:** For regular text content.

```html
<p>This is a paragraph of text. It can contain multiple sentences and will automatically wrap to new lines when needed.</p>
```

**Think of it as:** A paragraph in a book or essay.

### 5. `<img>` - Image
**What it is:** Displays pictures on your webpage.

**When to use:** When you want to show photos, graphics, or any visual content.

```html
<img src="photo.jpg" alt="Description of the image">
```

**Attributes explained:**
- `src` - The location/path of the image file
- `alt` - Description for screen readers and if image fails to load

**Think of it as:** A picture frame that holds your photos.

### 6. `<form>` - Form Container
**What it is:** A container for interactive elements that collect user input.

**When to use:** When you need users to submit information (login, contact forms, surveys).

```html
<form>
    <input type="text" placeholder="Enter your name">
    <input type="email" placeholder="Enter your email">
    <button type="submit">Submit</button>
</form>
```

**Think of it as:** A paper form that people fill out, but digital.

### 7. `<input>` - User Input Field
**What it is:** Interactive elements where users can type or select things.

**When to use:** Inside forms when you need user data.

**Common types:**
```html
<!-- Text input -->
<input type="text" placeholder="Your name">

<!-- Email input -->
<input type="email" placeholder="your@email.com">

<!-- Password input -->
<input type="password" placeholder="Password">

<!-- Checkbox -->
<input type="checkbox"> I agree to terms

<!-- Radio button -->
<input type="radio" name="color" value="red"> Red
<input type="radio" name="color" value="blue"> Blue

<!-- Submit button -->
<input type="submit" value="Send">
```

**Think of them as:** Different types of blanks to fill on a paper form.

## How These Work Together

Here's a simple example showing how these tags work together:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Website</title>
</head>
<body>
    <div>
        <h1>Welcome to My Blog</h1>
        
        <div>
            <h2>About Me</h2>
            <p>Hi! I'm <span>John</span>, and this is my personal blog.</p>
            <img src="profile.jpg" alt="John's profile picture">
        </div>
        
        <div>
            <h2>Contact Me</h2>
            <form>
                <p>Name: <input type="text" placeholder="Your name"></p>
                <p>Email: <input type="email" placeholder="Your email"></p>
                <p><input type="submit" value="Send Message"></p>
            </form>
        </div>
    </div>
</body>
</html>
```

## Key Points to Remember

1. **HTML tags are like labels** - they tell the browser what each piece of content is
2. **Most tags come in pairs** - opening tag `<div>` and closing tag `</div>`
3. **Structure matters** - organize your content logically with headings and containers
4. **Always use semantic tags** - choose tags based on meaning, not appearance
5. **Test your HTML** - make sure it displays correctly in browsers

HTML is the foundation of all websites. Master these basic tags, and you'll be able to create the structure for any webpage!
