# How to run an A/B test

### Create an A/B test

You can run an A/B test to see how a modular change will work from Modular Pages.

### Before you start...

Keep in mind that it isn't possible to create an A/B test without coordinating with the Digital Analytics team, since the purpose of an A/B test is to be able to measure the results. Firebase must be used to measure these results.

### Steps to follow to create an A/B Test in Modular Pages

**Step 1**. First, you'll need to have A/B Test creation permission in the CMS. If you don't, ask the NOC for it <img src="https://confluence.tid.es/s/24eubp/9012/15522zw/_/images/icons/emoticons/wink.svg" alt="(wink)" data-size="original">. You can also ask your OBPM or reference contact at Novum for assistance.

{% hint style="info" %}
This permission is not activated by default, so don't worry if you DON'T have the permission if you've never requested it 🙋🏾
{% endhint %}

**Step 2**. Access Modular Pages and edit the page where you want to include the test.

**Step 3**. In the **Content** step, search for the module you want to test. Click on the module sub-menu and select the **A/B Test** option

<figure><img src=".gitbook/assets/iniciarABTest.png" alt=""><figcaption></figcaption></figure>

**Step 4**. Add the name of the test. The **Key name** is the name that will be used in Firebase to identify the test. Then, click **Continue**.

<figure><img src=".gitbook/assets/FirebaseKey.png" alt=""><figcaption></figcaption></figure>

**Step 5.** A module editing window will open up when you enter the Key name. This is a replica of the module for which you are running the A/B test. Make changes pertaining to the test and click **OK**.

<figure><img src=".gitbook/assets/A_BTestCreado.png" alt=""><figcaption></figcaption></figure>

As you can see, another module has now been created. The two modules are identified as A and B, with A being the reference module (the source module, which is already in production) and B being the module to be tested (also called Variant A in the Firebase tool).

**Step 6.** **IMPORTANT**. The changes will be brought to PROD once you click on **Continue** in step **2 Content**. You can then finish publishing the entire Modular Page in step 3.

![(estrella roja)](https://confluence.tid.es/s/24eubp/9012/15522zw/\_/images/icons/emoticons/star\_red.svg) **IMPORTANT** ![(estrella roja)](https://confluence.tid.es/s/24eubp/9012/15522zw/\_/images/icons/emoticons/star\_red.svg)

Until the test is launched in Firebase, the app user will continue to see what is in production, i.e. the reference module, regardless of whether the test has already been configured in Modular Pages. It is therefore vitally important to coordinate with the Digital Analytics team so that you know when the test will first appear. The good news is that you can leave this ready in the Modular Pages CMS for when Digital Analytics can activate it in Firebase.

### Steps to mark the winning option in Modular Pages

The A/B test has finished the results are available in Firebase. Now what?

**Step 1**. Once the data has been analysed and you have made a decision on the winning module, access the Modular Pages CMS where the A/B test is running and edit the page containing the test.

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

**Step 2**. Click on the winning module's sub-menu and select **Set as winner**.

<figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>



**Step 3.** A summary window will appear showing the winning module and a preview. Confirm the change by clicking **Set as Winner**. Once you do this, the discarded module will be removed.

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

**Step 4**. **IMPORTANT**. The changes will be brought to PROD once you click on **Continue** in step **2 Content**.

In step **3 Overview**, you need to click **Save and publish**.

A window will open up in which you can indicate a description for the change you are going to make. Click **Confirm** to finish the setup.

### Good practices

You must create a ticket describing the test for the Digital Analytics team. You must also coordinate with the team, as there is no point in having an A/B test configured in Modular Pages if that test does not start from Firebase.

[Template Test A/B: \[OB\] Test A/B name](https://confluence.tid.es/pages/viewpage.action?pageId=141016807)
