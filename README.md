# Libanswers-styles

Back up the CSS and JS for NYU Libraries' instance of SpringShare's LibAnswers (LA) product:
[NYU Libraries LibAnswers](https://library.answers.nyu.edu/)

# Editing LibAnswers Code
There are two approaches to backup or modify the NYU Libraries' LibAnswers instance:

## Option 1: Editing the FAQ Groups Template
- Step 1: Access the LibAnswers Admin Interface
Login: Sign into your LibAnswers admin account.

Navigation: Locate the Admin section where you can edit page templates. 

- Step 2: Locate the FAQ Groups Template
Find the Template: Look for the specific FAQ Page template that is being used.

Reference Material: Optionally, review [this video](https://go.screenpal.com/watch/cTeIqCn18Kc) for a visual guide on the steps.

- Step 3: Edit the FAQ Page Template Code
Open the Template Editor: Click to edit the FAQ page template.

- Step 4: Save and Test
Save Your Changes: Commit the updated template by saving the file.

Clear Caches: If applicable, clear your browser or site cache to ensure that the latest version of the FAQ page is loaded.

Review the Page: Navigate to the live FAQ page to verify the changes. Ensure that the page is working as intended and that there are no layout issues.

## Option 2: Overriding with Custom CSS and HTML `style` tag
- Step 1: Access the LibAnswers Admin Interface
Login: Sign into your LibAnswers admin account.

Navigate: Go to your specific FAQ Group settings. You can access this by visiting [the URL](https://library.answers.nyu.edu/admin/groups/369/general) provided for your FAQ Group’s general settings panel.

- Step 2: Locate the `Look & Feel` Section
Look for the Customization Options: Find the “Look & Feel” panel.

Open the CSS Editor: This should allow you to insert custom styles that will override the default styling.

Step 3: Add the Custom CSS
Insert the Rule: Copy and paste the following CSS code into the editor:

```
<style>
span.s-la-faq-owner {display: none;}
</style>
```

- Step 4: Save and Verify
Save Changes: Commit the CSS update in your admin panel.

Test the Front End: Refresh your FAQ page to make sure that the element is hidden. You might also need to clear your browser cache or perform a hard refresh (Ctrl+F5 or Cmd+Shift+R) to see the update.
