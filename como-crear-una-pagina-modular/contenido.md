# Content

The content of a modular page is configured by inserting modules, choosing the order in which said modules appear on the page, and configuring the sections in which they are contained.

This step is divided into two parts:

- On the **left**-hand side are the **modules, which are arranged** as you want them to appear in the app.
- On the **right**-hand side is a **preview** of what the user will see in the app, which is as accurate as possible.

{% hint style="info" %} You should note that, in addition to what you see in the preview on the right-hand side, the modules can be configured to be shown to users based on a series of premises, including the intended audience. Therefore, what you see in the preview is not necessarily what the user will see.

If you want to see exactly how a modular page will appear for a certain user, you can run a [Test](../como-probar-el-contenido.md). {% endhint %}

The page is divided into two parts: a **Header** section, which you'll always see when creating a new page, and the rest of the page, which, depending on how you want to organize the content, may contain one or more sections.

## How to create a section

To create a new section, simply click **+New section** and fill in the fields as required in the window that opens.

<figure><img src="../.gitbook/assets/NewSectionWindow.png" alt=""><figcaption></figcaption></figure>

**Internal name**. This field is for internal use and allows you to correctly identify and differentiate each section of the modular page. It is a required field.

💡Try to make the name as descriptive as possible, as this will help you know what type of modules there are and what information is contained in the section.

### Design

In this tab, you need to select the section background color. Use the **Background color** dropdown menu to do so.

### Content

In this tab, you need to configure the section fields that will be seen by the app user.

<figure><img src="../.gitbook/assets/section_content.png" alt=""><figcaption></figcaption></figure>

- **Section title (optional)**. Choose the section title that will be seen by the app user when they see the modular page that you are creating or editing. It is an optional field and will therefore not be displayed if the field is left empty.

{% hint style="success" %} A section may or may not have a section title. Likewise, the content (modules) of the section will only appear when they apply to the user. {% endhint %}

- **Section description (optional)**. Describe the content of the section. This description will be seen by the app user. It is an optional field.
- **No link**. Option selected by default. It indicates that the section will not contain a link.
- **With link**. Select this option to add a link to the section.
    - **Link text action**. Indicate the link text.
    - **Select type URL**:
        - **URL**. Select this option to manually fill in the following **URL** field.
        - **Preconfigured**. Select this option to select one of the pre-configured URLs in the URL field.

<figure><img src="../.gitbook/assets/section_URL.png" width="563" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %} **Why aren't I seeing the section that I just configured in the preview?**

Until a section contains at least one module, it will not be shown in the preview of the modular page that you are creating or editing.

This is exactly how a modular page behaves for the app user. If a section has modules but none of them apply to the user, this section will not be shown to said user. This is even true if the section has modules and contains a section title, description and/or link. {% endhint %}

## How to add a module

Modules are always contained within a section. Therefore, before adding a module, you have to [create at least one section](contenido.md#como-crear-una-seccion). If you need to include a module in the **Header**, that section is always created by default.

Click **+Add module** within the section where you want to include a module.

- **Select module**. Select the module you are going to add.
- **Module ID**. The system will provide you with a unique ID for the module that you are adding. You can change the module ID as long as you don't use a name that is already in use.

<figure><img src="../.gitbook/assets/New_Module.png" alt=""><figcaption></figcaption></figure>

Consult the catalog of modules available from the CMS itself. Click on **Module catalog** on the main screen.

Do you need more information about how to consult the **Module catalog** ? 👇🏼

{% content-ref url="../catalogo-de-modulos-disponibles.md" %} [catalogo-de-modulos-disponibles.md](../catalogo-de-modulos-disponibles.md) {% endcontent-ref %}

### Module editing structure

Depending on the module you choose to add, the fields allowing additional configuration in the CMS will be displayed. To make it easier for you, these fields are divided into tabs according to their type:

#### Content

All fields related to the module content are available in this tab.

{% hint style="info" %} Remember that these fields will vary depending on the type of module that you add, and that some modules allow greater configurability than others 😉. {% endhint %}

If the module that you add has a specific CMS, you'll have a direct link that allows you to edit it.

<figure><img src="../.gitbook/assets/CMSpropio.png" alt=""><figcaption></figcaption></figure>

If you make changes to the module, you will need to refresh it in order to get a more accurate preview. Click <img src="../.gitbook/assets/image%20(4).png" data-size="line" alt=""> to refresh the information.

{% hint style="warning" %} 🚨 This user guide does not cover each field that can be edited in a given module, as this will depend on the added content. {% endhint %}

#### Audience

If you need to, you can configure the audiences for whom the module you are creating should appear from this tab.

You can use the audience composer to define the conditions that the user must meet in order to view the module.

<figure><img src="../.gitbook/assets/Audience.png" alt=""><figcaption></figcaption></figure>

Click **+Add condition** to add a new condition.

- Select **Is** in the drop-down menu to indicate that the audience does meet the condition
- Select **Not** in the drop-down menu to indicate that the audience does not meet the condition
- In the **Audience** drop-down menu, select the appropriate audience.

{% hint style="success" %} If you do not select **any audience**, the module will be visible to **all users**. {% endhint %}

#### Tracking

This tab allows you to configure the required tracking fields. Many of the fields are already tracked automatically, but you can also add these fields:

- **module_id (optional)**. Open text field related to the module ID that addresses Universal Analytics tracking*
- module_name (optional). Open text field related to the name of the module that addresses Universal Analytics tracking*

**Field that will become obsolete when Universal Analytics disappears.*

- **Content group (optional)**. Select one of the available groups in the drop-down menu.
- **Content category (optional)**. The values ​​that you can select in the **Content category** drop-down menu will be determined by your selection in the **Content group** drop-down menu.

**Analytics tracking preview**. Use this option to preview the tracking of the elements and their default values. Click on the module preview for the elements whose tracking you want to preview.

<figure><img src="../.gitbook/assets/PreviewTracking.gif" alt=""><figcaption></figcaption></figure>

Click **x Closing preview** to stop seeing this information and navigate to other tabs in the editing window.

#### QA

Tab that allows you to introduce a specific ID of the module to be used in the automatic or manual tests conducted by the QA team.

**Testing ID (optional)**. The testing team uses this field to check the information displayed on the screen.

It's usually fine to leave this field empty 🤓.

Click **OK** in the module creation/editing window once you have filled out all the necessary fields.

{% hint style="danger" %} **IMPORTANT**: remember that changes are not saved until you reach the last step, where you can choose to publish the changes or save them for later.

You will lose all the changes you have made if you close the screen at this point. {% endhint %}

---

## Common actions when creating/editing a page

Before detailing which common actions you can carry out within a modular page, remember that there are always secondary actions in both the section and the module.

Click <img src="../.gitbook/assets/image%20(3).png" data-size="line" alt=""> to open the sub-menu.

<figure><img src="../.gitbook/assets/menu_secundario%20(1).png" alt=""><figcaption></figcaption></figure>

### Moving a module within a section

Use the *Drag&amp;Drop* option to move the module to the desired position.

<figure><img src="../.gitbook/assets/move_module_in_the_same_section.gif" alt=""><figcaption></figcaption></figure>

### Moving a module to another section

Use the *Drag&amp;Drop* option to move the module to the desired position. You also have the **Move to another section** sub-menu. A window will open up in which you can indicate the section you want to move it to. Click **Move module** to confirm the move to the section indicated. The module will then be placed last in that section.

<figure><img src="../.gitbook/assets/move_to_another_section.png" alt=""><figcaption></figcaption></figure>

### Deactivating/Activating a module

Deactivating a module means that it won't be visible to app users. Likewise, activating it will make it visible again.

😉 Remember that when you deactivate a module it will not appear in the preview on the right-hand side.

Deactivating a module is less destructive than deleting it. If you delete it and subsequently want to recover it, you'd have to add it again and configure it from scratch.

Use the switch next to the module to activate/deactivate it:

<figure><img src="../.gitbook/assets/activardesactivar.png" alt=""><figcaption></figcaption></figure>

### Creating a group of alternative modules

It will sometimes be necessary for one module to be shown at a certain place in the app to some audiences and another module to be shown to others. This can be achieved through alternative modules. These modules work as if they were a single module i.e., several modules are configured, but only the one that applies to the user is shown.

The order of the alternative modules is important since the system will evaluate the first module that applies to the user. That will be the module that is shown.

<figure><img src="../.gitbook/assets/image%20(7).png" alt=""><figcaption><p>Example of alternative modules</p></figcaption></figure>

#### How to create a group of alternative modules

First of all, one of the modules will need to be placed in a section. Then, click on that module's sub-menu and select **+Add alternative**.

<figure><img src="../.gitbook/assets/image%20(8).png" alt=""><figcaption></figcaption></figure>

Configure the new alternative module and repeat the process for as many alternative modules are required.

{% hint style="warning" %} Note that only one module can contain no audience, and that this module must be placed in the last position. Otherwise, the condition of the other modules will never be evaluated. {% endhint %}

### Creating an A/B test

From modular pages, it is possible to run an A/B test to see how a module change will work.

You can find all the necessary information below 👇🏼

{% content-ref url="../como-hacer-un-test-a-b.md" %} [how-to-run-an-a-b-test.md](../como-hacer-un-test-a-b.md) {% endcontent-ref %}

---

Once you've finished configuring all of the content on the page, click **Continue** to go to the next step.

{% hint style="success" %} Remember that changes are not saved automatically, and you'll need to get to the last step to save or publish the changes. 🤓 {% endhint %}
