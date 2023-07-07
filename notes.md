## [Introduction to Site Building](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building)
* Sites are a fundamental component of Liferay DXP. Essentially, a Site is a collection of pages that contains content applications that provide additional functionality.

### Creating Sites
* You can create a Site from an existing Site Template, which includes a predefined set of pages with applications, or you can create a blank Site and build it from the ground up.
* Pages are just as flexible. Create a page from an existing page type or create one from one of the default page templates, or a page template you’ve created yourself.
* Sites and pages can be organized hierarchically.
* You can share content and pages between sites with the import and export options.
* Pages can be automatically added to a navigation menu when they’re created. You can hide pages if you prefer, or configure Page permissions restrict user access.
* **Liferay DXP also provides tools to enable you to make changes to your site without disrupting user experience. Liferay Sites can be staged, allowing changes to be made and tested on a site before being published to users. Liferay DXP’s Publications feature handles this for you. You can use Publications to develop, track, and update your Site in a safe environment, without affecting the live site that your users see.**

### Displaying Content
* Liferay DXP’s Content Management System (CMS) offers a variety of tools to create, manage and display content of many types (e.g. blogs, images, web content articles). 
* You can use the Web Content Display widget to display web content articles of your choosing.
* If you want to publish a mix of content types you can use the Asset Publisher or Displaying Collections. 
* You can manually select the content the Asset Publisher displays, or **you can have it display assets dynamically based on specific criteria**, giving you a great deal of control over the experience your users have. 
* You can also embed content from other websites with the Iframe widget or by creating an Embedded Page.
* **You can create and edit content inline with Fragments. Fragments are individual pieces of code (CSS, HTML, and JavaScript) that you can arrange and combine to build a page.** Several Fragments are included out-of-the-box that you can modify to create your content. If you require a more custom solution, you can create your own.
* Each piece of content has a default landing page, but you can create a Display Page Template to customize it. A Display Page Template maps portions of the Web Content (title, main body, image, etc.) to Fragments, so you can create the look you want.

### Personalizing User Experiences
* Liferay DXP’s Personalization and Segmentation framework lets you build site experiences that **respond to and meet your users interests and needs.** You can create user Segments based on specific criteria, such as the Organizations they belong to or their Role in the Site, and then **use it to display personalized page layouts and content for the user demographic, or you can integrate with Analytics Cloud to analyze the behavior of the users within the Segment to see how they interact with your Site**. You can even recommend content based on a user’s behavior.

### Customizing and Configuring Sites
* Sites and their Content can be easily localized to multiple languages as needed.
* The look and feel of your site can be changed by using different themes. Themes can be downloaded and deployed from Liferay Marketplace, or you can create a theme yourself. Themes determine the overall look and feel for a Site and define the CSS, JavaScript, and HTML for the page (via FreeMarker[^1] templates).
  
[^1]: FreeMarker combines standard HTML elements and provides the added benefit of variables, conditional statements, looping, and more. See Developing Themes for more information.

### Optimizing Sites
* Liferay DXP provides multiple tools and features for optimizing your Site, from increasing your Site’s Search Engine Optimization (SEO) ranking, to creating responsive pages optimized for each device, to honing your messaging campaigns with A/B Testing[^2].

[^2]: A/B Testing compares the current default variation of a page with the page variant(s) to see which pages perform better for a given goal (bounce rate, clicks, etc.). This enables you to make better, data-driven decisions about your site, so you can serve users and customers faster than ever before.

## [Adding a Site](https://learn.liferay.com/w/dxp/site-building/sites/adding-a-site)
* Steps that teach ow to create a Site (capital S because we are refering to a Liferay-specific terminology).
* Liferay Organizations enable distributed User management, providing a convenient way to organize and manage instance users and roles to reflect your organizational hierarchy. **Once an organization is created, you can also enable a dedicated Site for your Organization to facilitate distributed portal administration.** This feature is available for both parent and child Organizations, so you can quickly create a hierarchy of Sites with content created, administered, and tailored specifically to each group’s needs.
  > NOTE: (admonition here)
You can only use the blank template or custom templates when creating an Organization Site. **You cannot use other default templates.**
* Liferay User Groups are lists of users that can span multiple Organizations and Sites. You can create dedicated Sites for User Groups to add Pages to the personal Site of each group member. See User Group Sites for more information.

## [Site Templates](https://learn.liferay.com/w/dxp/site-building/sites/site-templates)
* Liferay provides Site Templates for designing structures and content that you can use during Site creation. Each template includes most standard Site applications for adding Pages, Stylebooks, Web Content, and more. 
* **Sites created with a template inherit all of its data.**
> NOTE: Site Templates support all Site applications **except Staging, Workflow, Memberships, Teams, and Segments.**
* Once you’ve created a Site using a template, you can make changes to the template’s Pages and automatically propagate those changes to connected Sites. See Propagating Template Changes for more information.
> IMPORTANT: Site Templates are primarily intended for maintaining Pages across multiple Sites. **If you need to create and maintain Web Content and other assets across Sites, use Asset Libraries.** 

## [Creating Site Templates](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/creating-site-templates)
* Teaches how to create a Site Template and talks about the options in the *New Site Template Menu*.
* With Site Templates, you can design and configure templates for creating Sites. Each template is built using the same tools as Sites.
* The UI for designing the template is identical with the UI for designing Sites. Just open the Site Template Menu (Site Menu) to access available applications and begin adding Style Books, Page Templates, Pages, and more.
*  (related to previous IMPORTANT admonition. The first part is the same, but there is this additional content on this page) If automatic propagation is not necessary for your use case, you can export and import Site data to transfer it between environments.
>  **IMPORTANT: Pages inherited from a template cannot be deleted. You also cannot directly add child Pages to them on the Site level. They can only be added or removed in the Site Template.**