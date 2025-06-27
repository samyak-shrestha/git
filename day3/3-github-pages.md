🏠 [Homepage](../README.md)

# GitHub Pages

#### **Steps to Create a Personal Website with GitHub Pages**

1.  **Create a GitHub Account**
    
    -   If you don’t have one, sign up at [github.com](https://github.com/).
2.  **Create a Repository for Your Website**
    
    -   Go to your GitHub dashboard.
    -   Click **New Repository**.
    -   **Name the repository** in this format: `username.github.io` (replace `username` with your actual GitHub username).
    -   Make sure the repository is public, and click **Create Repository**.
3.  **Add Files to Your Repository**
    
    -   You can either upload files directly to GitHub or clone the repository locally.
    -   If you’re coding locally, clone your repository with:

    ```bash
    git clone https://github.com/username/username.github.io.git
    ``` 
        
    -   Add an `index.html` file as your homepage. Here’s a basic template:
        
        ```
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>My Personal Website</title>
        </head>
        <body>
            <h1>Welcome to My Personal Website</h1>
            <p>This is a simple personal website hosted on GitHub Pages.</p>
        </body>
        </html>
        ```
        
2.  **Push Your Files to GitHub**
    
    -   If you’re working locally, after adding your `index.html`, push the changes to GitHub:
        
        
        ```bash
        git add .

        git commit -m "Initial website"

        git push origin main

        ``` 
        
3.  **Enable GitHub Pages**
    
    -   Once your files are uploaded, go to the repository’s settings.
    -   Scroll down to the **GitHub Pages** section.
    -   Under **Source**, select the **main** branch and save.
    -   Your website will now be live at `https://username.github.io/`.
4.  **Customizing Your Website**
    
    -   You can add more pages like `about.html` or style your site using CSS by adding a `style.css` file.
    -   Push changes to GitHub like any other repository.
5.  **Check Your Website**
    
    -   Open your browser and navigate to `https://username.github.io/`. Your personal website should be live!
  ---
### **Advantages of Using GitHub Pages**

1.  **Free Hosting**
    
    -   GitHub Pages is free, allowing you to host personal websites or project documentation without any cost.
2.  **Easy to Set Up**
    
    -   It’s simple for developers familiar with Git and GitHub to set up a website quickly without needing a hosting provider.
3.  **Custom Domain**
    
    -   You can link a custom domain to your GitHub Pages site if you prefer not to use `username.github.io`.
4.  **Version Control**
    
    -   Since GitHub Pages is integrated with Git, all your website’s code and changes are version controlled, making it easy to revert to previous states.
5.  **Great for Static Sites**
    
    -   GitHub Pages is optimized for static websites, such as portfolios, documentation, or blogs using static site generators like Jekyll.
6.  **SSL by Default**
    
    -   GitHub Pages provides HTTPS for your site out of the box, ensuring a secure connection.

----------

### **Disadvantages of Using GitHub Pages**

1.  **Limited to Static Sites**
    
    -   GitHub Pages does not support server-side code (like PHP, Node.js, or databases). You’re limited to static HTML, CSS, and JavaScript.
2.  **Basic Customization**
    
    -   While GitHub Pages is powerful for simple static websites, if you want advanced features (e.g., dynamic content or complex backend services), you’ll need to look elsewhere.
3.  **Lack of Built-in Analytics**
    
    -   GitHub Pages doesn’t provide analytics out of the box. You’ll need to integrate Google Analytics or another tool manually.
4.  **Performance for Complex Sites**
    
    -   If your site grows in complexity with lots of media files, GitHub Pages may not be the best for high-performance needs compared to dedicated hosting services.
5.  **Limitations in Storage and Bandwidth**
    
    -   There are soft limits on the size of repositories and bandwidth usage, which could be restrictive for larger projects.

----------

Using GitHub Pages is a great choice for personal portfolios, project documentation, or simple blogs. It’s a solid platform to quickly set up a personal website, especially for developers. However, for more complex websites or dynamic applications, you might need to explore other options.

🏠 [Homepage](../README.md)