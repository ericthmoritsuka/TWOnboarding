## Table of Contents
- [Table of Contents](#table-of-contents)
- [Introduction to Site Building](#introduction-to-site-building)
  - [Creating Sites](#creating-sites)
  - [Displaying Content](#displaying-content)
  - [Personalizing User Experiences](#personalizing-user-experiences)
  - [Customizing and Configuring Sites](#customizing-and-configuring-sites)
  - [Optimizing Sites](#optimizing-sites)
- [Adding a Site](#adding-a-site)
- [Site Templates](#site-templates)
- [Creating Site Templates](#creating-site-templates)
- [Propagating Template Changes](#propagating-template-changes)
  - [Which Template Changes are Propagated?](#which-template-changes-are-propagated)
  - [Enabling and Disabling Propagation](#enabling-and-disabling-propagation)
  - [Reconnecting Inherited Pages to Their Template](#reconnecting-inherited-pages-to-their-template)
- [Configuring Site Template Propagation](#configuring-site-template-propagation)
- [Exporting/Importing Site Templates](#exportingimporting-site-templates)
- [Site Hierarchies](#site-hierarchies)
  - [Content Sharing Between Sites](#content-sharing-between-sites)
  - [Site Hierarchy Roles and Permissions](#site-hierarchy-roles-and-permissions)
  - [Navigating Site Hierarchy with the Sites Directory Application](#navigating-site-hierarchy-with-the-sites-directory-application)
- [Site Membership](#site-membership)
- [Adding Members to Sites](#adding-members-to-sites)
  - [Managing Site Membership](#managing-site-membership)
  - [Joining Sites with the My Sites Application](#joining-sites-with-the-my-sites-application)
- [Invinting Members to Your Site](#invinting-members-to-your-site)
- [Creating Teams for Sites](#creating-teams-for-sites)
- [Personal Sites](#personal-sites)
  - [Profile Pages and Dashboard Pages](#profile-pages-and-dashboard-pages)
  - [Personal Site Permissions and Roles](#personal-site-permissions-and-roles)
  - [Customize Personal Sites with Portal Properties](#customize-personal-sites-with-portal-properties)
- [Exporting/Importing Site Pages and Content](#exportingimporting-site-pages-and-content)
  - [Site LAR Properties and Requirements](#site-lar-properties-and-requirements)
  - [Exporting Site Pages and Content](#exporting-site-pages-and-content)

---

## [Introduction to Site Building](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building)
* Sites are a fundamental component of Liferay DXP. Essentially, a Site is a collection of pages that contains content applications that provide additional functionality.

### [Creating Sites](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building#creating-sites)
* You can create a Site from an existing Site Template, which includes a predefined set of pages with applications, or you can create a blank Site and build it from the ground up.
* Pages are just as flexible. Create a page from an existing page type or create one from one of the default page templates, or a page template you’ve created yourself.
* Sites and pages can be organized hierarchically.
* You can share content and pages between sites with the import and export options.
* Pages can be automatically added to a navigation menu when they’re created. You can hide pages if you prefer, or configure Page permissions restrict user access.
* **Liferay DXP also provides tools to enable you to make changes to your site without disrupting user experience. Liferay Sites can be staged, allowing changes to be made and tested on a site before being published to users. Liferay DXP’s Publications feature handles this for you. You can use Publications to develop, track, and update your Site in a safe environment, without affecting the live site that your users see.**

### [Displaying Content](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building#displaying-content)
* Liferay DXP’s Content Management System (CMS) offers a variety of tools to create, manage and display content of many types (e.g. blogs, images, web content articles). 
* You can use the Web Content Display widget to display web content articles of your choosing.
* If you want to publish a mix of content types you can use the Asset Publisher or Displaying Collections. 
* You can manually select the content the Asset Publisher displays, or **you can have it display assets dynamically based on specific criteria**, giving you a great deal of control over the experience your users have. 
* You can also embed content from other websites with the Iframe widget or by creating an Embedded Page.
* **You can create and edit content inline with Fragments. Fragments are individual pieces of code (CSS, HTML, and JavaScript) that you can arrange and combine to build a page.** Several Fragments are included out-of-the-box that you can modify to create your content. If you require a more custom solution, you can create your own.
* Each piece of content has a default landing page, but you can create a Display Page Template to customize it. A Display Page Template maps portions of the Web Content (title, main body, image, etc.) to Fragments, so you can create the look you want.

### [Personalizing User Experiences](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building#personalizing-user-experiences)
* Liferay DXP’s Personalization and Segmentation framework lets you build site experiences that **respond to and meet your users interests and needs.** You can create user Segments based on specific criteria, such as the Organizations they belong to or their Role in the Site, and then **use it to display personalized page layouts and content for the user demographic, or you can integrate with Analytics Cloud to analyze the behavior of the users within the Segment to see how they interact with your Site**. You can even recommend content based on a user’s behavior.

### [Customizing and Configuring Sites](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building#customizing-and-configuring-sites)
* Sites and their Content can be easily localized to multiple languages as needed.
* The look and feel of your site can be changed by using different themes. Themes can be downloaded and deployed from Liferay Marketplace, or you can create a theme yourself. Themes determine the overall look and feel for a Site and define the CSS, JavaScript, and HTML for the page (via FreeMarker[^1] templates).
  
[^1]: FreeMarker combines standard HTML elements and provides the added benefit of variables, conditional statements, looping, and more. See Developing Themes for more information.

### [Optimizing Sites](https://learn.liferay.com/w/dxp/site-building/introduction-to-site-building#optimizing-sites)
* Liferay DXP provides multiple tools and features for optimizing your Site, from increasing your Site’s Search Engine Optimization (SEO) ranking, to creating responsive pages optimized for each device, to honing your messaging campaigns with A/B Testing[^2].

[^2]: A/B Testing compares the current default variation of a page with the page variant(s) to see which pages perform better for a given goal (bounce rate, clicks, etc.). This enables you to make better, data-driven decisions about your site, so you can serve users and customers faster than ever before.

---

## [Adding a Site](https://learn.liferay.com/w/dxp/site-building/sites/adding-a-site)
* Steps that teach ow to create a Site (capital S because we are refering to a Liferay-specific terminology).
* Liferay Organizations enable distributed User management, providing a convenient way to organize and manage instance users and roles to reflect your organizational hierarchy. **Once an organization is created, you can also enable a dedicated Site for your Organization to facilitate distributed portal administration.** This feature is available for both parent and child Organizations, so you can quickly create a hierarchy of Sites with content created, administered, and tailored specifically to each group’s needs.
  > NOTE: (admonition here)
You can only use the blank template or custom templates when creating an Organization Site. **You cannot use other default templates.**
* Liferay User Groups are lists of users that can span multiple Organizations and Sites. You can create dedicated Sites for User Groups to add Pages to the personal Site of each group member. See User Group Sites for more information.

---

## [Site Templates](https://learn.liferay.com/w/dxp/site-building/sites/site-templates)
* Liferay provides Site Templates for designing structures and content that you can use during Site creation. Each template includes most standard Site applications for adding Pages, Stylebooks, Web Content, and more. 
* **Sites created with a template inherit all of its data.**
> NOTE: Site Templates support all Site applications **except Staging, Workflow, Memberships, Teams, and Segments.**
* Once you’ve created a Site using a template, you can make changes to the template’s Pages and automatically propagate those changes to connected Sites. See Propagating Template Changes for more information.
> IMPORTANT: Site Templates are primarily intended for maintaining Pages across multiple Sites. **If you need to create and maintain Web Content and other assets across Sites, use Asset Libraries.** 

---

## [Creating Site Templates](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/creating-site-templates)
* Teaches how to create a Site Template and talks about the options in the *New Site Template Menu*.
* With Site Templates, you can design and configure templates for creating Sites. Each template is built using the same tools as Sites.
* The UI for designing the template is identical with the UI for designing Sites. Just open the Site Template Menu (Site Menu) to access available applications and begin adding Style Books, Page Templates, Pages, and more.
*  (related to previous IMPORTANT admonition. The first part is the same, but there is this additional content on this page) If automatic propagation is not necessary for your use case, you can export and import Site data to transfer it between environments.
>  **IMPORTANT: Pages inherited from a template cannot be deleted. You also cannot directly add child Pages to them on the Site level. They can only be added or removed in the Site Template.**

---

## [Propagating Template Changes](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/propagating-template-changes)
* When Site Template propagation is enabled, **you can make changes to the template’s Pages and automatically propagate those changes to connected Sites. **
  * Making changes to a Site Page inherited from a template prevents the propagation of template changes to that Page. To restore propagation for the Page, you must discard changes made to it in the Site. 
  * If you’ve edited multiple inherited Pages and you’d like to restore propagation from the Site Template, you must reset changes for each one individually.
> NOTE: By default, propagation is triggered for each connected Site individually, when it is first visited by a user after changes are made. However, you can configure your system to also trigger propagation to connected Sites simultaneously whenever users toggle a template to Ready for Propagation.

### [Which Template Changes are Propagated?](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/propagating-template-changes#which-template-changes-are-propagated)
* **Only changes to a template’s Pages and Page elements are propagated to connected Sites.** This includes newly created Pages as well as any changes to fragments and widgets in existing Pages.
* **Other application data is only copied at initial Site creation; subsequent changes are not automatically propagated.**
* This part was mentioned in other pages, but it is important here as well: Site Templates are primarily intended for **maintaining Pages across multiple Sites.** If you need to create and maintain Web Content and other assets across Sites, use Asset Libraries.

### [Enabling and Disabling Propagation](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/propagating-template-changes#enabling-and-disabling-propagation)
* When creating a template, you determine whether to enable or disable automatic propagation, but you can change this setting at any time.
* Alternatively, you can enable or disable automatic propagation via the Site Templates application page. Just click the Actions button (Actions Button) for the desired template and select Disable Propagation or Ready for Propagation.
* Teaches how to enable/disable propagation.

### [Reconnecting Inherited Pages to Their Template](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/propagating-template-changes#reconnecting-inherited-pages-to-their-template)
* (As explained above) If you make changes to a Site Page inherited from a template, it is disconnected from the template’s Page and is not automatically propagated. To reconnect the Site Page to the template, you must discard your changes to the Site Page.
* Teaches how to discard changes to a Site Page and resync with its template.
> WARNING: Resetting changes reverts any changes made to the Site Page directly. This can result in data loss. Proceed with caution.

---

## [Configuring Site Template Propagation](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/configuring-site-template-propagation)
* By default, site template changes are propagated automatically to a connected site when a user visits the site after the template is updated. 
* You can configure an additional manual trigger that propagates to all connected sites simultaneously. To enable manual propagation, use the Trigger Propagation setting. When enabled, clicking the *Ready for Propagation* button in the site template editor triggers propagation to all connected sites. 
* Enabling this setting does not stop the automatic propagation of template changes that occurs when users visit connected sites.
> IMPORTANT: Automatic propagation can be resource intensive, depending the scope of changes made to a template.
* Teaches how to configure Site Template propagation.
* If propagation is disabled for a Site Template, enabling propagation immediately begins propagating changes to connected Sites simultaneously. While propagation remains enabled for the template, subsequent changes are propagated to sites individually when they’re first visited by a user.

---
## [Exporting/Importing Site Templates](https://learn.liferay.com/w/dxp/site-building/sites/site-templates/exporting-importing-site-templates)
* Teaches how to export/import individual site templates.
* Teaches how to Bulk Export/Import
* With Bulk Exports, you cannot configure the Pages and content included for each template. 
* Unlike individual exports, you can determine whether Page Templates are included in your export.
* With Bulk Imports, you can determine whether Page Templates included in the LAR file are imported with the Site Templates.

---

## [Site Hierarchies](https://learn.liferay.com/w/dxp/site-building/sites/site-hierarchies)
*  Sites can be organized hierarchically, just like Organizations, with child Sites. 
*  Organizing Sites hierarchically lets you share content between them easily. 
*  The difference between Sites and Organizations is that **Sites organize pages, content, application data, and Users (via site memberships)**, whereas **Organizations only group Users**.

### [Content Sharing Between Sites](https://learn.liferay.com/w/dxp/site-building/sites/site-hierarchies#content-sharing-between-sites)
*  Content sharing is available for Sites within the same hierarchy. 
> You can share these content types across Sites: Web Content Structures, Web Content Templates, Document Types, Vocabularies and Categories, Widget Templates, Data Definitions (Dynamic Data Lists)

### [Site Hierarchy Roles and Permissions](https://learn.liferay.com/w/dxp/site-building/sites/site-hierarchies#site-hierarchy-roles-and-permissions)
* Each child site in the hierarchy has its own Administrator
* The Site Administrator Role permissions don’t flow down to child Sites in the hierarchy
* If a Site Administrator creates a child Site, he or she has the same permissions in that child Site. This is because creating a Site makes you the owner of that Site (not inheritance).
* A Site Administrator has no default Role in any child Sites created by other Site Administrators.
> NOTE: If you want a User to have administrative access to all Sites in a Site/child Site hierarchy, you must create a Role based on the Site Administrator Role that has the permission Manage Subsites.

### [Navigating Site Hierarchy with the Sites Directory Application](https://learn.liferay.com/w/dxp/site-building/sites/site-hierarchies#navigating-site-hierarchy-with-the-sites-directory-application)
* The Sites Directory application is a configurable app that **shows a hierarchy of Sites and child Sites. It enables Users to navigate to any of the displayed Sites.**
* Teaches how to access Sites Directory

---

## [Site Membership](https://learn.liferay.com/w/dxp/site-building/sites/site-membership)
* Being a member of a Site grants users access and abilities beyond an unauthenticated guest user. 
* Site members have more permissions than guests for many widgets like Message Boards and Wikis that enable them to create content and collaborate on your Site.
* Site members can be associated with Roles that grant Site privileges.
* Site Roles are created at a global level, but **when they’re assigned they only provide permissions for the specific Site where they were assigned.**
* Since Roles are created at a global level, **they can’t be created by Site Administrators** (since Site Administrators only have Administrator privileges for their Site). 
* Teams let Site Administrators assign permissions to groups of Users within their Sites. 

---

## [Adding Members to Sites](https://learn.liferay.com/w/dxp/site-building/sites/site-membership/adding-members-to-sites)
* Sites are where all your content and pages are stored, and Users access and create that content.

### [Managing Site Membership](https://learn.liferay.com/w/dxp/site-building/sites/site-membership/adding-members-to-sites#managing-site-membership)
* Administrators can manage Site members from that Site’s Site Membership page.
* ***There is a lack of information on how to get to Memberships. At least, I had a hard time finding it, maybe it could be rewritten to make it easier to find?***
* Teaches how to add and remove members.
* Teaches how to bulk remove Users.
* Teaches how to assign Site roles.
* ***Is it really necessary to add "Follow these steps to make an existing User a member of the Site:"(Don't introduce the steps directly underneath a heading - is it ok if I write a sentence like this?)***
* ***follow these steps: (Only use : after independent clauses)***
* ***Joining Sites with the My Sites Application (is the definite article The appropriate in this case? Couldn't it be omitted since the possessive adjective My is also being used?)***
* ***In the title it is called My Sites Application, in the body it is called My Sites Directory application***

### [Joining Sites with the My Sites Application](https://learn.liferay.com/w/dxp/site-building/sites/site-membership/adding-members-to-sites#joining-sites-with-the-my-sites-application)

*  My Sites Directory application lists the Sites a User belongs to. This application is added to User Dashboard pages by default. You can view the available open and restricted Sites by adding the My Sites application to a page and accessing the Available Sites tab. You can request access to any of the Sites you’re not a member of by selecting the Site’s Options button (Options) and clicking Join.

---

## [Invinting Members to Your Site](https://learn.liferay.com/w/dxp/site-building/sites/site-membership/inviting-members-to-your-site)
* Teaches how to invite members to the site.
* ***How do I get to the widget?***
* Maybe break the information down a little more? It looks a little dense.
* Should the title be Inviting Members to Your site using the Invite Members widget (as it is specifically mentioning just this method?)

---

## [Creating Teams for Sites](https://learn.liferay.com/w/dxp/site-building/sites/site-membership/creating-teams-for-sites)
* If you have an ad hoc group of Users who perform the same set of tasks in a Site (moderating a site’s Wiki content, managing Message Boards threads, writing blogs, editing a specific page in the Site, etc.), you can organize them into Site Teams, and then assign the team permissions for various Site-specific functions.
* Site Teams are the preferred method for administering permissions within a single Site. 
* The permissions assigned to a Site Team **only apply to that Site.**
> NOTE: To create and apply permissions for a group of Users to use across multiple Sites or Organizations in your Liferay Portal instance, **consider aggregating the Users into a User Group and assigning the User Group permissions via Roles.**
* ***The steps below cover these topics: Adding a Team to a Site, Adding Members to a Team, Managing Team Permissions, Managing Team App Permissions (Is this necessary? could it be a paragraph, could I omit it?)***
* Teaches how to do the topics mentioned above.
* The path to get to Teams is better here than in [Adding Members to Site](https://learn.liferay.com/w/dxp/site-building/sites/site-membership/adding-members-to-sites#managing-site-membership).
> NOTE: You can configure other Site membership groupings, such as Users, Organizations, and User Groups in the Site Memberships app, which is also in the Members tab.
> NOTE: Setting permissions for the Team assigns those permissions to all the Team’s members. Only Administrators who can edit/manage the Team can manage Team permissions.
> You can also manage Team permissions from an app (Message Boards, for example). 

---

## [Personal Sites](https://learn.liferay.com/w/dxp/site-building/sites/personal-sites)
* By default, Liferay generates a personal site for every user. Each site includes two page sets: My Profile (public) and My Dashboard (private).
* You can disable or customize personal sites using portal properties
> IMPORTANT: For Liferay 7.4 U22+ and GA22+, new Liferay installations include a release feature flag **that disables the creation of Private Pages, including Dashboard Pages**. To manually create custom Dashboard Pages for a personal Site, Private Pages must be enabled for your Liferay system.
* ***should't the first topic be updated using the important admonition?***
> TIP: With User Group Sites, you can dynamically add Pages to the personal Sites of all group members. See User Group Sites for more information.

### [Profile Pages and Dashboard Pages](https://learn.liferay.com/w/dxp/site-building/sites/personal-sites#profile-pages-and-dashboard-pages)
* In Profile Pages, Users can share content (e.g., blog, activities) publicly. By default, each Profile Page displays the User’s basic information and provides a download link to the User’s vCard (virtual business card).
* In Dashboard Pages, user can access private files, create personalized RSS feeds, manage Site memberships, and more. By default, each Dashboard Page includes the My Sites widget.

### [Personal Site Permissions and Roles](https://learn.liferay.com/w/dxp/site-building/sites/personal-sites#personal-site-permissions-and-roles)
* Administrators can customize the modifiable portions of personal Sites through Liferay Portal’s permissions system by removing permissions from Roles (disallow all Users from modifying something by removing the relevant permission from the User Role).
* Users can administer their personal sites and modify the pages and applications when they are members of the Power User Role.

### [Customize Personal Sites with Portal Properties](https://learn.liferay.com/w/dxp/site-building/sites/personal-sites#customizing-personal-sites-with-portal-properties)
* There are several portal properties you can add to portal-ext.properties to customize the default pages of personal Sites. You can customize the names of the pages, the applications that appear on the pages, the themes and layout templates of pages, and more.
* There is a table with some functionalities and respective properties we can add to `portal.properties`
* The Public and Private Page Sets of personal Sites are handled separately. You can leave one Page Set enabled while disabling the other.
* If you initially had user personal Sites enabled for your instance but then disabled them, existing personal Sites remain on your instance until the next time users sign in, at which point they’re removed.

---

## [Exporting/Importing Site Pages and Content](https://learn.liferay.com/w/dxp/site-building/sites/exporting-importing-site-pages-and-content)
* Liferay Sites include the Export/Import applications for extracting and transferring Site data as Liferay Archive (LAR) files. You can access these tools at the Site level. (what is the site level?)
> NOTE: You can also access export and import functions for individual Site applications and Page widgets.

### [Site LAR Properties and Requirements](https://learn.liferay.com/w/dxp/site-building/sites/exporting-importing-site-pages-and-content#site-lar-properties-and-requirements)
* LARs are version dependent. **They can be imported into a Site on another Liferay server, as long as the Liferay versions on each server are the same.**
* Some naming conflicts are handled automatically. For example, **if the LAR you’re importing and the Site both have a page with the same friendly URL, a number is appended to the friendly URL and incremented until the conflict no longer occurs.** The same is true for category names.
* **You can use LARs to restore a Site, but you must delete your Site entirely and then create a new Site with the same name to import the LAR into.** This avoids potential data conflicts between content that exists both in the LAR and in the Site.
> IMPORTANT: Periodically exporting LARs is not a backup solution; it should only be used to migrate data between two environments. Please refer to the Backing up a Liferay Portal Installation to learn about backing up your Liferay installation.

### [Exporting Site Pages and Content](https://learn.liferay.com/w/dxp/site-building/sites/exporting-importing-site-pages-and-content#exporting-site-pages-and-content)

