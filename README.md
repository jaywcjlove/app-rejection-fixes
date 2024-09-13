App Rejection Fixes
===

This repository documents the various reasons why apps were rejected during the App Store review process and provides solutions to resolve these issues. It serves as a resource for developers to better understand common rejection scenarios and how to address them effectively, helping streamline the review process for future submissions.

## 🚫 Guideline 1.5 - Safety

1.5 Developer Information People need to know how to reach you with questions and support issues. Make sure your app and its Support URL include an easy way to contact you; this is particularly important for apps that may be used in the classroom. Failure to include accurate and up-to-date contact information not only frustrates customers, but may violate the law in some countries or regions. Also ensure that Wallet passes include valid contact information from the issuer and are signed with a dedicated certificate assigned to the brand or trademark owner of the pass.

**Q: Issue Description**

The Support URL provided in App Store Connect, https://wangchujiang.com/quick-rss/, does not direct to a website with information users can use to ask questions and request support.

> [!TIP]  
> **A: 💯 Rejection Fixes**
> 
> In most cases, including links and contact information for technical support passes the review without issues. However, occasionally a stricter reviewer may reject the app because of it. To solve this, I used a free solution by offering technical support through GitHub using the [issue](https://github.com/jaywcjlove/quick-rss/issues/new?assignees=&labels=support%2Cfeedback%2Cquestion&projects=&template=bug_report.yml&title=%F0%9F%99%8B%E2%80%8D%E2%99%82%EF%B8%8F+Support+%26+Feedback%3A+Quick+RSS) creation feature, and the app successfully passed the review.
> 
> <a href="https://github.com/jaywcjlove/quick-rss/issues/new?assignees=&labels=support%2Cfeedback%2Cquestion&projects=&template=bug_report.yml&title=%F0%9F%99%8B%E2%80%8D%E2%99%82%EF%B8%8F+Support+%26+Feedback%3A+Quick+RSS"><img src="https://github.com/user-attachments/assets/ec2e48e7-fbcc-404d-969a-a5729354aad4" alt="Rejection Fixes" width="360" /></a>

## 🚫 Guideline 2.1 - Performance - App Completeness

Submissions to App Review, including apps you make available for pre-order, should be final versions with all necessary metadata and fully functional URLs included; placeholder text, empty websites, and other temporary content should be scrubbed before submission. Make sure your app has been tested on-device for bugs and stability before you submit it, and include demo account info (and turn on your back-end service!) if your app includes a login. If you are unable to provide a demo account due to legal or security obligations, you may include a built-in demo mode in lieu of a demo account with prior approval by Apple. Ensure the demo mode exhibits your app’s full features and functionality. We will reject incomplete app bundles and binaries that crash or exhibit obvious technical problems.

**Q: Issue Description**

The app exhibited one or more bugs that would negatively impact App Store users.

Bug description: No content was displayed on the PASS Purchase page.

> [!WARNING]  
> **A: 💯 Rejection Fixes**
> 
> ???

## 🚫 Guideline 2.3 - Performance - Accurate Metadata

We noticed that your app’s metadata includes the following information, which is not relevant to the app’s content and functionality:

What’ new text showed iOS reference.

**Q: Next Steps**

To resolve this issue, please revise or remove this content from your app’s metadata. For resources on metadata best practices, you may want to review the App Store Product Page information available on the Apple Developer website.

> [!TIP]  
> **A: 💯 Rejection Fixes**
> 
> While mentioning macOS in the release notes for an iOS app is not problematic, mentioning iOS in the release notes for a macOS app is likely to result in rejection.

## 🚫 Guideline 2.4.5(i) - Performance

In order to continue reviewing your app, we require additional information.

Your app uses one or more entitlements which do not appear to have matching functionality within the app. Please reply to this message in App Store Connect and describe how and where the app uses the following entitlements. You will not need to upload a new binary to provide this information.

Apps should have only the minimum set of entitlements necessary for the app to function properly. If there are entitlements that are not needed, please remove them and submit an updated binary. You will need to Developer Reject the app to upload an updated version.

```
com.apple.security.files.bookmarks.app-scope
com.apple.security.network.server
```

> [!TIP]  
> **A: 💯 Rejection Fixes**
> 
> When using permissions, you need to include a note during the initial review. If not, the app might be rejected. In that case, simply respond with a description of where the permissions are used, and the issue will be resolved.

## 🚫 Guideline 4 - Design

We noticed an issue with your app's user interface that contributes to a lower-quality user experience than App Store users expect.

Specifically, we found that when the user closes the main application window there is no menu item to re-open it.

**Q: Next Steps**

It would be appropriate for the app to implement a Window menu that lists the main window so it can be reopened, or provide similar functionality in another menu item.

Alternatively, if the application is a single-window app, it might be appropriate to save data and quit the app when the main window is closed.

> [!TIP]  
> **A: 💯 Rejection Fixes**
> 
> Add a ‘Main Windows’ menu item to the Windows menu. This way, when the application is closed, users can click this menu item to reopen the main window.
> 
> <img src="https://github.com/user-attachments/assets/d316f9a4-c683-40cd-af25-93f357d6f80f" alt="Rejection Fixes" width="360" />
> 
> Alternatively, you can implement it so that clicking the close button exits the application directly.
