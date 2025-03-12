# Web Accessibility Project According to WCAG 2.2

This project aims to demonstrate how to improve web accessibility using WCAG 2.2 guidelines. The example HTML code has been modified to comply with A, AA, and AAA accessibility criteria, applying best practices such as ARIA attributes, semantic HTML5 tags, alternative text for images, and enhanced keyboard navigation.

## Objectives

- Modify an HTML file to be accessible according to WCAG 2.2 standards.
- Ensure the code meets A, AA, and AAA accessibility criteria.
- Use accessibility validation tools such as **WAVE**, **Axe**, and **Lighthouse**.
- Document the accessibility improvement process and code changes.

## Modifications Made

### 1. **Navigation Accessibility:**
   - **Change:** Added `role="link"` and `aria-label` attributes to navigation links.
   - **Objective:** Improve navigation link comprehension for assistive technology users.
   - **Example:**
     ```html
     <a href="index.html" role="link" aria-label="Go to Home">Home</a>
     ```

### 2. **HTML5 Semantic Tags:**
   - **Change:** Improved document structure using proper HTML5 tags such as `<header>`, `<main>`, `<section>`, and `<footer>`.
   - **Objective:** Enhance content organization and accessibility, making navigation easier for assistive technology users.
   - **Example:**
     ```html
     <header>
         <h1>Main Title</h1>
     </header>
     ```

### 3. **Images:**
   - **Change:** Added meaningful descriptions in the `alt` attribute of images.
   - **Objective:** Ensure images are accessible for visually impaired users.
   

### 4. **Form:**
   - **Change:** Added `aria-required="true"` to required form fields and used `aria-label` to describe fields.
   - **Objective:** Improve form accessibility, ensuring assistive technology users understand required fields.
   - **Example:**
     ```html
     <input type="text" id="name" name="name" aria-required="true" placeholder="Enter your name" aria-label="Field to enter name">
     ```

### 5. **Buttons and Actions:**
   - **Change:** Added `aria-label` attributes to buttons to better describe their functionality.
   - **Objective:** Improve button action comprehension.
   - **Example:**
     ```html
     <button onclick="alert('Hello!')" aria-label="Show alert message">Click Me</button>
     ```

### 6. **Keyboard Navigation Improvements:**
   - **Change:** Ensured that interactive elements, such as buttons and forms, are keyboard accessible.
   - **Objective:** Guarantee that keyboard-only users can interact with all page elements.

### 7. **Color Contrast:**
   - **Change:** Verified that the contrast between text and background is adequate for visually impaired users.
   - **Objective:** Ensure text is readable for all users.

## Validation Tools Used

- **WAVE:** [WAVE Web Accessibility Evaluation Tool](https://wave.webaim.org/)
- **Axe:** [Axe Accessibility Testing](https://www.deque.com/axe/browser-extensions/)
- **Lighthouse:** Built-in tool in Google Chrome DevTools.
- **Accessibility Insights:** Validation tool for accessibility testing.

## Validation Process

### Steps Taken:

1. **Initial Test:** The original code was validated using **WAVE** and **Axe**. Results showed multiple errors and warnings related to missing `alt` attributes, color contrast, and lack of ARIA attributes in forms.
2. **Code Modification:** Changes were applied to improve accessibility, such as adding ARIA attributes, using semantic tags, and improving form and button accessibility.
3. **Modified Version Validation:** After modifications, the code was re-tested with **WAVE** and **Axe** to ensure compliance with accessibility criteria.
4. **Iteration:** Additional refinements were made, such as adjusting color contrast and adding alternative text for images.

### Validation Results

- **Before Modification:** The original code had multiple warnings, mainly regarding missing `alt` attributes for images, color contrast, and lack of ARIA attributes in forms.
- **After Modification:** Validation tool results showed most warnings were resolved, and the code met **AA** WCAG 2.2 criteria. Keyboard navigation and comprehension of links and forms were also improved.

## Screenshots

Original Code and WAVE Validation Before Modification:
![alt text](image3.png) and ![alt text](image4.png)

Modified Code and WAVE Validation After Modification:
![alt text](image5.png) and ![alt text](image6.png)

## Conclusion

This project applied web accessibility best practices to enhance the usability and accessibility of an HTML page according to WCAG 2.2 guidelines. After iterating the code with multiple validation tools, compliance with **AA** accessibility criteria was achieved.

## Files Included in the Repository

- `index.html`: Original unmodified code.
- `index_modified.html`: Code modified according to WCAG 2.2 accessibility standards.
- `README.md`: Project documentation and validation process.
- Screenshots from accessibility validation tools.
