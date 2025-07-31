# Premium Dog Food Landing Page

This project is a landing page for a premium dog food brand, showcasing its key features, nutritional benefits, and health improvements for dogs.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Code Explanation](#code-explanation)
  - [HTML Structure](#html-structure)
  - [CSS Styling](#css-styling)

## Features

- **Hero Section**: Highlights the brand's unique selling proposition with a prominent title and a grid of key features.
- **Key Features Grid**: Displays four core features (Real Food, Made Fresh, Premium Ingredient, Vet Developed) surrounding a central image of a dog food bowl.
- **Call to Action (CTA)**: A clear button to encourage purchases, accompanied by payment information and a money-back guarantee.
- **Nutrition Section**: Details the nutritional benefits of the dog food with statistics and a secondary CTA.
- **Gastrointestinal Health Section**: Explains how the product improves digestive health.
- **Prebiotics Section**: Focuses on the role of prebiotics in supporting gut health.


## Technologies Used

- HTML5
- CSS3
- Google Fonts (Inter Tight)

## Setup Instructions

To run this project locally, follow these steps:

1.  **Clone the repository (if applicable):**
    ```bash
    git clone https://github.com/OfomiMatthew/gem-commerce-landing-page.git
    cd gem-commerce-landing-page
    ```
    

2.  **Create the directory structure:**
    Ensure you have the following folder structure:
    ```
    your-project-folder/
    ├── index.html
    ├── css/
    │   └── styles.css
    └── assets/
        └── images/
            ├── g6396.png
            ├── Group _1.png
            ├── Frame.png
            ├── Group.png
            ├── Page-1.png
            ├── shield-check.png
            ├── paypal.png
            ├── visa.png
            ├── mastercard.png
            ├── apple-pay.png
            ├── google-pay.png
            ├── dog_food.png
            ├── dog_2.png
            └── dog-kibble.png
    ```
    *Note: The image assets are crucial for the page's appearance. Make sure they are placed correctly in the `assets/images/` directory.* If you don't have these images, the page will still function but will have broken image links.

3.  **Open `index.html`:**
    Simply open the `index.html` file in your web browser. All styles will be automatically applied.

## Code Explanation

### HTML Structure

The `index.html` file defines the semantic structure of the landing page. It is divided into several key sections:

-   **`<!DOCTYPE html>`**: Declares the document type as HTML5.
-   **`<html lang="en">`**: The root element, specifying the document language as English.
-   **`<head>`**: Contains meta-information about the HTML document:
    -   `<meta charset="UTF-8">`: Specifies the character encoding for the document.
    -   `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Configures the viewport for responsive design.
    -   `<title>Premium Dog Food - Healthy Nutrition for Your Pet</title>`: Sets the title that appears in the browser tab.
    -   `<link rel="preconnect" ...>` and `<link href="..." rel="stylesheet">`: Links to Google Fonts (`Inter Tight`) and the external CSS stylesheet (`css/styles.css`).
-   **`<body>`**: Contains the visible content of the web page, structured into distinct sections:
    -   **Hero Section (`.hero-section`)**:
        -   `<h1>`: The main headline, emphasizing the brand's difference.
        -   `.features-grid`: A container for the feature cards and the central image, using CSS Grid for layout.
        -   `.feature-card`: Individual feature blocks (Real Food, Made Fresh, Premium Ingredient, Vet Developed), each with an icon, heading, and paragraph.
        -   `.central-image`: The main dog food bowl image positioned in the center of the features grid.
        -   `.cta-section`: Contains the primary call-to-action button and payment information.
        -   `.payment-info`: Displays the money-back guarantee and various payment method logos.
    -   **Nutrition Section (`.nutrition-section`)**:
        -   `<h2>`: Headline about nutrition being foundational.
        -   `<p>`: Descriptive text about supplements.
        -   `.key-points`: Contains statistical highlights about the dog food's effectiveness, each with a number and description.
        -   `<hr>`: Horizontal rules to separate stat items.
        -   `.cta-button-secondary`: A secondary call-to-action button.
        -   `.nutrition-image`: An image of a happy dog with food.
    -   **Gastrointestinal Health Section (`.gastrointestinal-section`)**:
        -   `<h2>`: Headline about improving gastrointestinal health.
        -   `<p>`: Explanatory text and customer feedback.
        -   `.gastrointestinal-image`: An image of two dogs eating.
    -   **Prebiotics Section (`.prebiotics-section`)**:
        -   `<h2>`: Headline about prebiotics.
        -   `<p>`: Explanatory text about prebiotics.
        -   `.prebiotics-image`: An image of dog food kibble.

### CSS Styling

The `css/styles.css` file provides the visual presentation and layout for the HTML elements. It uses a combination of modern CSS techniques, including Flexbox, CSS Grid, and media queries for responsiveness.

-   **Reset and Base Styles (`*`, `body`, `.container`)**:
    -   `*`: A universal reset to remove default margins and paddings and set `box-sizing` to `border-box` for easier layout management.
    -   `body`: Sets basic typography (font family, line height, color) and a light background color.
    -   `.container`: Defines a maximum width and horizontal centering for content, providing consistent padding on the sides.

-   **Hero Section Styling (`.hero-section`, `.hero-title`, `.features-grid`, `.central-image`, `.feature-card`, `.feature-icon`, `.cta-button`, `.payment-info`)**:
    -   `.hero-section`: Sets background, padding, and centers text.
    -   `.hero-title`: Styles the main headline with specific font size, weight, color, and line height.
    -   `.features-grid`: Utilizes `display: grid` to create a 3x3 grid layout. `grid-template-columns` and `grid-template-rows` define the column and row sizes. `position: relative` is used to allow precise positioning of child elements.
    -   `.central-image`: Positions the dog food bowl image in the center of the grid (`grid-column: 2; grid-row: 2;`). It's styled as a circle with `border-radius: 50%` .
    -   `.feature-card`: Styles individual feature cards, using `display: flex` for icon and text alignment. Specific classes like `.feature-top-left`, `.feature-top-right`, etc., use `grid-column`, `grid-row`, `justify-self`, and `align-self` to place them precisely around the central image within the grid.
    -   `.feature-icon`: Styles the circular background for each icon, with different background colors for visual distinction (`.icon-top-left`, `.icon-top-right`, etc.).
    -   `.cta-button`: Styles the primary call-to-action button with a distinct background color, text color, padding, and border-radius.
    -   `.payment-info`: Uses `display: flex` to arrange payment methods and guarantee text, with `justify-content: center` and `gap` for spacing.

-   **Nutrition Section Styling (`.nutrition-section`, `.nutrition-content`, `.nutrition-text`, `.key-points`, `.stat-item`, `.cta-button-secondary`)**:
    -   `.nutrition-section`: Sets background and padding.
    -   `.nutrition-content`: Uses `display: grid` with two columns (`1fr 1fr`) for a side-by-side layout of text and image.
    -   `.nutrition-text h2` and `p`: Styles the headlines and paragraphs within this section.
    -   `.key-points`: Contains the statistical items.
    -   `.stat-item`: Uses `display: flex` to align the statistic number and its description. The `hr` element is styled to be a simple separator.
    -   `.cta-button-secondary`: Styles the secondary call-to-action button, similar to the primary one but potentially with different sizing.

-   **Gastrointestinal and Prebiotics Sections Styling (`.gastrointestinal-section`, `.gastrointestinal-content`, `.prebiotics-section`, `.prebiotics-content`)**:
    -   These sections follow a similar grid layout pattern as the Nutrition Section, alternating the image and text positions for visual variety.
    -   Headlines (`h2`) and paragraphs (`p`) are styled consistently across these sections.


This CSS ensures that the landing page is visually appealing, providing a consistent user experience. 



