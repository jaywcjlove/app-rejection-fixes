App Rejection Fixes
===

This repository documents the various reasons why apps were rejected during the App Store review process and provides solutions to resolve these issues. It serves as a resource for developers to better understand common rejection scenarios and how to address them effectively, helping streamline the review process for future submissions.

## 🚫 Guideline 1.5 - Safety

1.5 Developer Information People need to know how to reach you with questions and support issues. Make sure your app and its Support URL include an easy way to contact you; this is particularly important for apps that may be used in the classroom. Failure to include accurate and up-to-date contact information not only frustrates customers, but may violate the law in some countries or regions. Also ensure that Wallet passes include valid contact information from the issuer and are signed with a dedicated certificate assigned to the brand or trademark owner of the pass.

**Q: Issue Description**

The Support URL provided in App Store Connect, https://wangchujiang.com/quick-rss/, does not direct to a website with information users can use to ask questions and request support.

**A: 💯 Rejection Fixes**

Add a ‘Main Windows’ menu item to the Windows menu. This way, when the application is closed, users can click this menu item to reopen the main window.

![Rejection Fixes](https://github.com/user-attachments/assets/d316f9a4-c683-40cd-af25-93f357d6f80f)

Alternatively, you can implement it so that clicking the close button exits the application directly.

## 🚫 Guideline 4 - Design

We noticed an issue with your app's user interface that contributes to a lower-quality user experience than App Store users expect.

Specifically, we found that when the user closes the main application window there is no menu item to re-open it.

**Q: Next Steps**

It would be appropriate for the app to implement a Window menu that lists the main window so it can be reopened, or provide similar functionality in another menu item.

Alternatively, if the application is a single-window app, it might be appropriate to save data and quit the app when the main window is closed.

**A: 💯 Rejection Fixes**